# Community Contribution Guidelines


## Introduction

Thank you for your interest in contributing to the INSPIRE Validator. We would appreciate it if you read this information carefully so that we can propagate your changes as soon as possible.

Please read and follow our [Code of Conduct](code_of_conduct.adoc) before you interact with the INSPIRE Validation community.

The aim of these contribution guidelines is to help INSPIRE Validator contributors to verify that their pull requests to the ETS repository and their helpdesk issues are properly submitted. These guidelines are designed to save time and hassle caused by improperly created pull requests or issues that have to be rejected and re-submitted. 



### How to submit your pull request to the [ETS repository](https://github.com/inspire-eu-validation/ets-repository)

First, please check that the following conditions apply:

* The improvement you would like to add has not been already developed nor is under current development (please refer to the changelog and release planning documents as well as the open issues in the helpdesk).

* The improvement is not already available in the staging environment.



Afterwards, please follow these instructions:

1. Create a fork of the [staging branch](https://github.com/inspire-eu-validation/ets-repository/tree/staging) and write your code there.

2. Create a separate pull request to the [staging branch](https://github.com/inspire-eu-validation/ets-repository/tree/staging) for each single improvement made to the code.

3. Write a short description of the pull request. Please include the file (and/or the url) required to test the improvement made on the description of the pull request. This will help a lot to understand and test the changes made.

4. An expert from the JRC will also review the pull request and check that the changes are beneficial for the INSPIRE community.

5. You will be notified as soon as your contribution is published in the staging environment of the Validator.

6. Give us your feedback based on the implementation of the changes of your pull request in the staging environment. We would like to be sure that everything is working fine also for you.



### How to [report an issue](https://github.com/inspire-eu-validation/community/issues/new?template=problem.md)

Before reporting an issue in the [INSPIRE Validator helpdesk](https://github.com/inspire-eu-validation/community/issues/), please check the [list of known limitations](https://github.com/inspire-eu-validation/community/wiki/Known-limitations).



To help us investigate the issue, please include:



1. The full name of the test (conformance class) that generated the issue.

2. The resource or the link to the resource that you tested. If this has credentials, please send the credentials to inspire-helpdesk@bilbomatica.com.

3. A short description of the steps to reproduce your issue.

4. If possible, a screenshot illustrating the problem.

5. The browser and version used.



Please note that issues cannot be investigated for services/datasets that we cannot access.



### How to [suggest an improvement](https://github.com/inspire-eu-validation/community/issues/new?template=improvement-proposal.md)

Please create a brief summary of your improvement proposal, including:



* The rationale or motivation behind the proposal.

* The proposed change.

* Whether there is full or partial funding available for implementing the proposal.



To help us understand the proposal, please include:

1. A link to further information on the proposal.

2. Source code or code snippets.

3. Some diagrams, mockups or screenshots illustrating the proposal.



### How to [start a discussion](https://github.com/inspire-eu-validation/community/issues/new?template=discussion.md)

Please, make a short description about the topic you would like to discuss.





### Labeling conventions for [helpdesk issues](https://github.com/inspire-eu-validation/community/issues/)

These labels are assigned to the helpdesk issues by the helpdesk team. They will add the label as soon as one of them applies. Here is the list of available labels:



* **bug**: Something is not working.

* **enhancement**: New feature or request.

* **for-2017.4-discussion**: This issue will be discussed with the sub-group 2017.4.

* **under analysis**: A possible solution is under analysis.

* **question**: Further information is requested to the issue reporter.

* **planned**: A solution will be developed, the task has been scheduled.

* **under development**: The solution is under development.

* **ready for testing**: The solution was developed, deployed in the staging enviroment and waiting for testing and acceptance by the issue reporter.

* **solved**: The solution was tested and accepted by the issue reporter, but not yet deployed in the production instance.

* **deployed in reference validator**: The solution was deployed in the production enviroment.

* **wontfix**: This issue will not be worked on.
