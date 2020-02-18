# Table of contents
- [Introduction](#introduction)
- [Release Plan Objective and Summary](#release-planning-summary)
- [Overview](#overview)
  * [Current Situation](#current-situation)
  * [Desired Situation](#desired-situation)
- [Release Planning](#release-planning)
  * [v2020.1 - 15/03/2020](#v20201---15-03-2020)
  * [v2020.2 - 15/06/2020](#v20202---15-06-2020)
  * [v2020.3 - 15/09/2020](#v20203---15-09-2020)
  * [v2021.0 - 15/01/2021](#v20210---15-01-2021)
- [Release Delivery](#release-delivery)

# Introduction
This document illustrates the release planning strategy for the INSPIRE Reference Validator, including all its components (ATS, ETS and ETF). The document explains the rationale behind the plan and details the foreseen release dates throughout the year together with their main expected changes. It also lists a number of resources to inform users on the future expected changes in the INSPIRE Reference Validator and to check in detail the content of each release.


# Release Plan Objective and Summary
The objective of this document is to explain the release planning process for the INSPIRE Reference Validator in an open, clear and transparent way to the INSPIRE community in order to ensure that stable validation criteria are provided and communicated efficiently. The release plan is beneficial to the whole INSPIRE community, in particular to the Member States data providers and implementers in preparation to the Monitoring process that will take place each year in December. 

The core of the release plan is the annual major release of the INSPIRE Reference Validator. This release includes the validation rules applied in the end-of-year Monitoring process, i.e. the tests against which the conformity of the INSPIRE resources published by Member States will be measured. In order to give INSPIRE data providers and implementers sufficient time to prepare their resources for the Monitoring deadline in December, each year the major release of the INSPIRE Reference Validator is published several months in advance (in June).

Therefore, the main idea of the release plan is to include all the _breaking-changes_ (i.e. changes which make tests more restrictive as well as new tests) in the versions of the INSPIRE Reference Validator released during the first half of the year (in January, March and June) and the _non-breaking-changes_ (i.e. changes which make tests less restrictive and changes to the interface, which do not impact the tests) in any version of the INSPIRE Reference Validator, including the one released during the second half of the year (in September). In addition, _hotfixes_ (i.e. fixes to major bugs or faults) are released as quickly as possible, even outside the planned releases.

The following schedule of versions is conceived in accordance with the objective of offering the version used in the annual report at mid-year, that can be used from that moment for the preparation of data aligned with the requirements to be met at the end of the year. This schedule refers to the remaining part of year 2020 and the beginning of year 2021, however the plan has to be seen as a generic plan that will also apply for the next years.
* **v2020.1 - 15/03/2020.** It includes a first batch of binding developments to the end-2020 report, as well as improvements to the ETF tool.
  * Breaking changes
  * Non-breaking changes
  * Hotfixes
* **v2020.2 - 15/06/2020.** This **v2020.2 release contains all the validations to be considered for the evaluation of the annual report.**
This version includes all the requirements and restrictions to incorporate the annual report, so that users can use it from this moment on to appropriately adapt their data until the end of the year. 
  * Breaking changes
  * Non-breaking changes
  * Hotfixes
* **v2020.3 - 15/09/2020.** This **v2020.3 version will be used for the evaluation of the annual report.**
The version published at this time contains all the restrictions and possible non-breaking changes or Hotfixes, that is to say developments that do not imply additional work for the report but that can lower the degree of restriction of the requirements or correct existing bugs.
  * Non-breaking changes
  * Hotfixes
* **v2021.b - 15/09/2020.** In addition, a version will be published that incorporates the changes to be evaluated in the following year's report, so that those community members who want to test them will have it at their disposal.
  * Breaking changes
  * Non-breaking changes
  * Hotfixes
* **v2021.0 - 15/01/2021.** After the conclusion of the reporting cycle, a first version of the ATS/ETS and the ETF to be used in the 2021 reporting cycle will be published in the production environment.
From this version onwards, the same release philosophy will be followed, so that the community has a clear understanding of what is to be released, the functionalities offered and the scope of these developments.
  * Breaking changes
  * Non-breaking changes
  * Hotfixes

# Overview
## Current Situation
The INSPIRE Validation & conformity testing framework consists of Abstract and Executable Testsuites, of the ETF framework and User Interface and of additional tools such as the Linkage Checker. It helps INSPIRE implementers to understand whether their data sets and network services are compliant to the technical guidance. Resources need to fulfill a wide set of requirements to qualify as fully compliant.
The framework was initially made available in 2016 and has since given data providers feedback to implement the requirements correctly. Before the initial availability of the framework, there was often a lot of ambiguity in what exactly is compliant and what not, which reduced interoperability. In 2019, the INSPIRE monitoring was first based on direct harvesting and compliance testing of data sets, network services and metadata. This is a first step to continuous, data driven monitoring, with fewer manual steps and corrections applied by intermediate SDIs. 
As of late 2019, the monitoring for 2019 has just been completed, and implementers have relied heavily on the framework and associated tools to make their resources fit for INSPIRE. 

## Desired Situation
When reviewing the current situation, there are some aspects that would help to make conformity testing a more straightforward task. To support both INSPIRE implementers and the central reporting optimally, it is proposed the following for the INSPIRE validation and conformity testing framework:
* Create transparency into Release Planning process and into deployment states
* Provide stable conformity criteria with enough lead time before the monitoring period
* Communicate changes and their impact to the community on a regular basis

In this way, this document sets out a transparent proposal for planning the various releases of the INSPIRE Reference Validator.

# Release Planning
At the core of the release planning strategy is the annual major release. This is the release that encompasses the rules that will be applied in the end-of-year reporting. To give tool developers and INSPIRE implementers sufficient time to adjust, this release will be made with significant lead time to the monitoring period.

In order to provide users with an environment where developments can be adequately tested, different test environments are offered, where the ATS/ETS developed will be tested on a specific instance of the ETF.
There will be different instances of the ETF deploying different branches of the ATS/ETS/ETF set, with different purposes
* [Production instance](http://inspire.ec.europa.eu/validator/): stable deployment with official and proven ATS/ETS for the current year's report
* [Staging instance](http://staging-inspire-validator.eu-west-1.elasticbeanstalk.com/etf-webapp/): which will contain a pre-publication version of the production
* Beta instance (this instance is not available yet): this environment will contain a version corresponding to the following year's compliance requirements, so users can choose to validate against the current year's version or the following year's version

The different versions to be released may contain different developments, both at the ATS/ETS and ETF level. The following classification of functionalities to be incorporated is established according to the relevance of the changes introduced in each development, as well as to the impact they have on the validations to be carried out.
* Breaking changes:
  * Corresponding to an implementation that makes the compliance more restrictive and difficult to pass
  * New tests
* Non-Breaking changes:
  * Implementation reducing restriction for the correct compliance in a requirement
  * Minor changes to the interface that add new functionalities to the interface but it has no effect on the tests
* Hotfix:
  * Detected bug that needs to be implemented and extended as soon as possible to the different instances

In order to facilitate reporting at the end of the year, a fundamental aspect is that the community is adequately informed of the versions to be released, as well as being given enough time to accommodate the data to be reported on a stable, unvarying and reliable version.
Globally, a work schedule is established for the annual report in which the focus is mainly on concentrating the breaking-changes in the first half of the year, so that by June of each year, there is a stable version on which to test the data and where the changes introduced up to the end of the year do not impact more restrictively on the validations to be made on the reporting information.
Thus, the following schedule of versions can be conceived in accordance with the objective of offering the version used in the annual report at mid-year that can be used from that moment for the preparation of data aligned with the requirements to be met at the end of the year.
* **v2020.1 - 15/03/2020.** It includes a first batch of binding developments to the end-2020 report, as well as improvements to the ETF tool.
* **v2020.2 - 15/06/2020.** This **v2020.2 release contains all the validations to be considered for the evaluation of the annual report.**
This version includes all the requirements and restrictions to incorporate the annual report, so that users can use it from this moment on to appropriately adapt their data until the end of the year. 
  * Breaking changes
  * Non-breaking changes
  * Hotfixes
* **v2020.3 - 15/09/2020.** This **v2020.3 version will be used for the evaluation of the annual report.**
The version published at this time contains all the restrictions and possible non-breaking changes or Hotfixes, that is to say developments that do not imply additional work for the report but that can lower the degree of restriction of the requirements or correct existing bugs.
* **v2021.b - 15/09/2020.** In addition, a version will be published that incorporates the changes to be evaluated in the following year's report, so that those community members who want to test them will have it at their disposal.
* **v2021.0 - 15/01/2021.** After the conclusion of the reporting cycle, a first version of the ATS/ETS and the ETF to be used in the 2021 reporting cycle will be published in the production environment.
From this version onwards, the same release philosophy will be followed, so that the community has a clear understanding of what is to be released, the functionalities offered and the scope of these developments.

These announced versions must be orchestrated not only in terms of infrastructure and deployment environments, but also in terms of managing the various branches in the community repository.
Thus, in order to clarify the operation between the different branches and the deployment environments where the ATS/ETS will be able to be run, the diagrams below are included:

## v2020.1 - 15/03/2020
This first version v2020.1 to be deployed in the production instance on 15/03/2020 includes breaking-changes, i.e. new requirements and developments that directly impact in the report to be made. 
As it can be seen, it is based on the master branch, which is deployed in production environment.
All issues that come in the period prior to the release, whether they are breaking changes, non-breaking changes or Hotfixes will be deployed as soon as they have been developed in the staging environment, as usual. 
If a Hotfix needs to be incorporated in the production instance before the release date, the production deployment will be updated.
Finally, according to the planned date, the validated developments will be taken from the staging branch, creating the branch v2020.1 that will be merged in the master branch and deployed in the production environment. 
This way, the reference version from this moment becomes v2020.1.

![v2020.1](./img/v2020.1.png "v2020.1")

## v2020.2 - 15/06/2020
As mentioned above, the first part of the year will focus on developing and consolidating the requirements for the annual report.
Thus, version v2020.2 contains all the breaking changes, non-breaking changes and Hotfixes needed to generate a version on which to test the annual report. This version guarantees that, if the validations are successfully passed, the report will also be successful, since the final version to be used for the evaluation of the report (v2020.3) will not incorporate changes that imply more requirements or greater restrictions to the reported data.

![v2020.2](./img/v2020.2.png "v2020.2")

## v2020.3 - 15/09/2020
This v2020.3 version will be used for the 2020 report. Version v2020.3 will include non-breaking changes and Hotfixes, which guarantees that the data tested with version v2020.2 will successfully pass the validations contained in v2020.3. Furthermore, in any case, version v2020.3 will only incorporate developments that facilitate the report, thus benefiting users from all the work done since version v2020.2.
Additionally,  version 2021.b will also be released in the beta instance, which will incorporate the first breaking changes for the 2021 report. 
This version will be available to be used in advance by the community for the preparation of the 2021 report.

![v2020.3](./img/v2020.3.png "v2020.3")

## v2021.0 - 15/01/2021
Version 2021.0 is the first release of the year and is established as the basis for the 2021 report. It incorporates breaking changes, non-breaking changes and Hotfixes as a baseline for the following developments to be made in the 2021 report.

![v2021.0](./img/v2021.0.png "v2021.1")

Thus, by means of the presentation of these diagrams, the schedule in terms of versions and branches for the next year is shown, always having as a priority the establishment of a version as a baseline by the middle of the year to be able to consolidate the report with enough time in advance.

As mentioned above, this release schedule has been made to cover an annual cycle as an example, but this release schedule is intended to be established consistently over time.

# Release Delivery
The release of a version involves the generation of certain artifacts so that the community has access to all the assets generated and can clearly identify the elements that are released.
Thus, the release of a new version implies acting on the following elements.
* Github release. A release v202x.y.z (dd/mm/yyyy) is generated, including:
  * New Features, listed and grouped by ATS, ETS and ETF
  * Bugfixes, listed and identified by issue, description and pull request
  * Enhancements, listed and identified by issue, description and pull request
  * Documentation, pointing to the various documents produced for the generated version
  * Assets, code packages are generated to facilitate the deployment to users, containing
	  * ets-repository, zip file containing the ets-repository corresponding to the created branch
   * etf-release-v202x.y.z, containing ETF deployment instructions and artifacts
	  * source code, zip file containing the community repository for the delivered version  
* GitHub packages. A GitHub package is generated including the instructions and elements for the ETF deployment corresponding to the version released through the use of Docker.
* Branches management. The following branches should be managed, according to the specific purpose of the version, depending on the time of year and the changes it incorporates (breaking changes, non-breaking changes or Hotfixes).
  * branch v202x.y.z , this branch is created from the next branch, which includes all the developments made according to the criteria established for the specific version
  * master is synchronized with the branch generated for the specific version
  * next, is the branch that generates the version and is only merged by another branch in version v202x.0 where it is overwritten by the beta branch
  * beta, is created from version v202x.2 and updated with breaking changes, non-breaking changes and Hotfixes
* Issues management. Issues related to the release must be properly managed according to the following actions: 
  * Assign the corresponding milestone: v202x.y.z
  * Update the corresponding label: deployed in reference validator
  
