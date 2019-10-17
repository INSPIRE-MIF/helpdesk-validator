# Steps for API usage

We will be using cURL code as examples for the usage of the API. This can be translated to any programming language to automatize API calls. All the documentation on the API can be found at http://inspire.ec.europa.eu/validator/swagger-ui.html.
## Check the Status of the service

`curl -X GET \
  http://inspire.ec.europa.eu/validator/v2/status`

```
{
    "name": "ETF",
    "status": "GOOD",
    "heartbeat": "1570453763953",
    "willExpireAt": "1570453923953",
    "version": "2.0.0-b190624T1219",
    "uptime": "577371",
    "allocatedMemory": "864071264",
    "presumableFreeMemory": "13581898144",
    "totalSpace": "9223372036853727232",
    "freeSpace": "9223372031888719872",
    "cpuLoad": "0.000125"
}
```

## Locate the TestSuite id for the test run

`curl -X GET http://inspire.ec.europa.eu/validator/v2/ExecutableTestSuites`

```
{
    "EtfItemCollection": {
        "version": 2.0,
        "returnedItems": 64,
        "position": 0,
        "ref": "http://inspire.ec.europa.eu/validator/v2/ExecutableTestSuites.json?&offset=0&limit=1500",
        "executableTestSuites": {
            "ExecutableTestSuite": [
                {
                    "id": "EID59692c11-df86-49ad-be7f-94a1e1ddd8da",
                    "remoteResource": "https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/2.0",
                    "label": "Common Requirements for ISO/TC 19139:2007 based INSPIRE metadata records.",
                    .
                    .
                    .
```

We check the key `ExecutableTestSuites` to get the list of all the ETS. Each of them is represented as an object. Using the `label` key we locate the ETS, and get the `id` key.

## Create a new TestObject to upload the file to test

`curl -X POST 'http://inspire.ec.europa.eu/validator/v2/TestObjects?action=upload' -F fileupload=@[PATH/TO/LOCAL/FILE]`

```
{
    "testObject": {
        "id": "EID844c4c8c-ab7a-4104-b94b-4607921119c5"
    },
    "files": [
        {
            "name": "xml.metadata.get.xml",
            "size": "24625",
            "type": "application/xml"
        }
    ]
}
```
We indicate the location of the file to upload in the `-F` option. In the response, we check the `id` key. This option can be used to test metadata files or datasets, in a single file or in a zipped tile.

## Create a new TestRun using the TestSuite id and the TestObject ID

`curl -X POST http://inspire.ec.europa.eu/validator/v2/TestRuns -d '{"label":"Metadata test with uploaded TestObject","executableTestSuiteIds":["EID59692c11-df86-49ad-be7f-94a1e1ddd8da"],"arguments":{"files_to_test":".*","tests_to_execute":".*"},"testObject":{"id":"EID844c4c8c-ab7a-4104-b94b-4607921119c5"}}'`

```
{
    "EtfItemCollection": {
        "version": 2.0,
        "returnedItems": 1,
        "ref": "http://inspire.ec.europa.eu/validator/v2/TestRuns/e7653a13-4235-4254-bc50-eaddbb587053.json",
        "testRuns": {
            "TestRun": {
                "id": "EIDe7653a13-4235-4254-bc50-eaddbb587053",
                "status": "UNDEFINED",
                "label": "Metadata test with uploaded TestObject",
                "defaultLang": "en",
                "startTimestamp": "2019-10-07T13:31:25.821Z",
                .
                .
                .
```
We use both IDs previously generated, from the TestSuite and the uploaded TestObject, and create a new TestRun indicating the ID for them in the list `executableTestSuites` and in the `testObject`, respectively.

This will return the TestRun with the `status` (that would be `UNDEFINED` in the first place as it has not yet been executed). With the TestRun `id` we can check periodically if the TestRun has finished or not.

## Checking the results

`http://inspire.ec.europa.eu/validator/v2/TestRuns/EIDe7653a13-4235-4254-bc50-eaddbb587053`

```
{
    "EtfItemCollection": {
        "version": 2.0,
        "returnedItems": 1,
        "ref": "http://inspire.ec.europa.eu/validator/v2/TestRuns/e7653a13-4235-4254-bc50-eaddbb587053.json",
        "testRuns": {
            "TestRun": {
                "id": "EIDe7653a13-4235-4254-bc50-eaddbb587053",
                "status": "UNDEFINED",
                "label": "Metadata test with uploaded TestObject",
                "defaultLang": "en",
                "startTimestamp": "2019-10-07T13:31:25.821Z",
                "testTasks": {
                    "TestTask": {
                        "id": "EIDb6da9149-aff5-4d0b-b940-ea4f325934c1",
                        "parent": {
                            .
                            .
                            .
```

Using the ID from the TestRun creation's response, we can access the test report. Using the previous URL plus `.html`, we can get the same report accessible from the webapp.

If we want to process the results automatically, we can use the key `testRuns.TestRun.status` to check the global result, or use the items `testRuns.TestRun.testTasks.TestTask` and for each element in this list, get `testTaskResult.ref` key, to get the key of each test task in the TestSuite, and execute the call

`http://inspire.ec.europa.eu/validator/v2/TestTaskResults/[TEST_TASK_ID].[json|xml|html]`

```
{
    "EtfItemCollection": {
        "version": 2.0,
        "returnedItems": 1,
        "ref": "http://inspire.ec.europa.eu/validator/v2/TestTaskResults/6822b3a6-e019-4862-9c9a-0f31e8dcb125.json",
        "testTaskResults": {
            "TestTaskResult": {
                "id": "EID6822b3a6-e019-4862-9c9a-0f31e8dcb125",
                "testObject": {
                    "ref": "EID1508643f-6dc4-4407-8e62-dc0e2ca8b4f5"
                },
                "testModuleResults": {
                    "TestModuleResult": {
                        "id": "EID049ebfac-976f-4ee8-b5c0-12fcb4980e6a",
                        "testCaseResults": {
                            "TestCaseResult": [
                                .
                                .
                                .
```

and get the individual steps for this TestSuite.
