# Table of contents
- [Introduction](#introduction)
- [Objective and Summary](#objective-and-summary)
- [Release Planning](#release-planning)
  * [Instances of the INSPIRE Reference Validator](#instances-of-the-inspire-reference-validator)
  * [Annual releases](#annual-releases)
    * [v2020.1 - 15/03/2020](#v20201---15-03-2020)
    * [v2020.2 - 15/06/2020](#v20202---15-06-2020)
    * [v2020.3 - 15/09/2020](#v20203---15-09-2020)
    * [v2021.0 - 15/01/2021](#v20210---15-01-2021)
- [Release Delivery](#release-delivery)

# Introduction

This document illustrates the release planning strategy for the INSPIRE Reference Validator, including all its components (ATS, ETS and ETF). The document explains the rationale behind the plan and details the foreseen release dates throughout the year together with their main expected changes. It also lists a number of resources for users to get informed on the future expected changes (future releases) in the INSPIRE Reference Validator and to check in detail the content of each released version (past releases).

# Objective and Summary

The objective of this document is to explain the release planning process for the INSPIRE Reference Validator in an open, clear and transparent way to the INSPIRE community in order to ensure that stable validation criteria are provided and communicated efficiently. The release plan is beneficial to the whole INSPIRE community, in particular to Member States data providers and implementers in preparation to the Monitoring process that takes place each year in December and makes use of the INSPIRE Reference Validator.

The core of the release plan is **the annual major release** of the INSPIRE Reference Validator. This release includes the validation rules applied in the end-of-year Monitoring process, i.e. the reference tests against which the conformity of the INSPIRE resources published by Member States are measured. In order to give INSPIRE data providers and implementers sufficient time to prepare their resources for the Monitoring deadline in December, each year the major release of the INSPIRE Reference Validator is published several months in advance (in June). In addition to this major release, every year **a number of minor releases** are also published (in January, March and September).

In particular, all the **_breaking changes_** (i.e. changes which make tests more restrictive as well as new tests) are only included in the versions of the INSPIRE Reference Validator released during the first half of the year (in January, March and June), while the **_non-breaking changes_** (i.e. changes which make tests less restrictive as well as changes to the interface, which do not impact the tests) are included in any version of the INSPIRE Reference Validator (in January, March, June and September). In addition, **_hotfixes_** (i.e. fixes to major bugs or faults) are released as quickly as possible, even outside the planned releases.

# Release Planning

## Instances of the INSPIRE Reference Validator

Multiple instances of the INSPIRE Reference Validator are currently available (or will be made available) which have different purposes:

* [Production instance](http://inspire.ec.europa.eu/validator/): this is the reference instance used for validating INSPIRE resources in the end-of-year Monitoring process. It only includes the consolidated changes, i.e. changes which have been already tested and approved by the INSPIRE community. Releases of the INSPIRE Reference Validator (with the exception of beta releases) always refer to releases of the production instance.

* [Staging instance](http://staging-inspire-validator.eu-west-1.elasticbeanstalk.com/etf-webapp/): this instance includes all the latest changes to the INSPIRE Reference Validator, including new tests and new functionality, before these are also moved to the Production instance within a release. The Staging instance is only used for testing purposes by the INSPIRE community.

* Beta instance (available from Q3-2020): this instance, developed independently of the Production and Staging instances, includes the changes foreseen for the following year. It provides INSPIRE users with the possibility to test validation requirements foreseen for the following year already before the Monitoring deadline of the current year.

## Annual releases

As mentioned above, several releases of the INSPIRE Reference Validator are scheduled each year with the main goal of concentrating breaking changes in the first half of the year in order to produce the major release used for the end-of-year Monitoring process already in June. The scheduled annual releases are described in detail in the next sub-sections. In addition to the different infrastructure and deployment environments, the different releases are managed using different branches of the [_ets-repository_ repository](https://github.com/inspire-eu-validation/ets-repository).

For simplicity, the descriptions make explicit reference to releases in the years 2020/2021, but the same release schedule will be applied consistently over the following years:

* **v2020.1 - 15/03/2020**: it includes both breaking and non-breaking changes.
* **v2020.2 - 15/06/2020**: it includes both breaking and non-breaking changes.
* **v2020.3 - 15/09/2020**: it only includes non-breaking changes, so that any INSPIRE resource passing the test in the previous release automatically passes the same test in this release. This release is the one used for the end-of-year Monitoring process.
* **v2021.b - 15/09/2020**: it includes both breaking and non-breaking changes which are planned to become effective (for Monitoring purposes) in the following year.
* **v2021.0 - 15/01/2021**: it includes both breaking and non-breaking changes, including those available in the beta instance of the previous year.

### v2020.1 - 15/03/2020
This release is scheduled for 15/03/2020 and includes breaking and non-breaking changes. All these changes (each managed in a dedicated branch) are first incorporated in the _staging_ branch, i.e. they are made available in the Staging instance, and afterwards also in the _v2020.1_ branch. This branch is finally merged into the _master_ branch, which will make all changes available in the Production instance. Should hotfixes be needed at any time, they are immediately incorporated both in the _staging_ and the _master_ branches.

![v2020.1](./img/v2020.1.png "v2020.1")

### v2020.2 - 15/06/2020
This release is scheduled for 15/06/2020 and includes breaking and non-breaking changes. All these changes (each managed in a dedicated branch) are first incorporated in the _staging_ branch, i.e. they are made available in the Staging instance, and afterwards also in the _v2020.2_ branch. This branch is finally merged into the _master_ branch, which will make all changes available in the Production instance, and also in the _beta_ branch. Should hotfixes be needed at any time, they are immediately incorporated both in the _staging_ and the _master_ branches. <!-- check how hotfixes are addressed: is there a need to create a v.2020.1.1 branch? If yes, update description. -->

![v2020.2](./img/v2020.2.png "v2020.2")

### v2020.3 - 15/09/2020
This release is scheduled for 15/09/2020 and only includes non-breaking changes. All these changes (each managed in a dedicated branch) are first incorporated in the _staging_ branch, i.e. they are made available in the Staging instance, and afterwards also in the _v2020.3_ branch. This branch is finally merged into the _master_ branch, which will make all changes available in the Production instance. Conversely, in addition to the non-breaking changes, breaking changes (each managed in a dedicated branch) are also incorporated in the _beta_ branch. Should hotfixes be needed at any time, they are immediately incorporated both in the _staging_, the _master_ and the _beta_ branches. <!-- check how hotfixes are addressed: is there a need to create a v.2020.2.1 branch? If yes, update description. -->

![v2020.3](./img/v2020.3.png "v2020.3")

### v2021.0 - 15/01/2021
This release is scheduled for 15/01/2021 and includes breaking and non-breaking changes. All these changes (each managed in a dedicated branch) are progressively incorporated in the _beta_ branch, and finally also in the _v2021.0_ branch. This branch is finally merged into the _staging_ and the _master_ branches, which will make all changes available in both the Staging and the Production instances. Should hotfixes be needed at any time, they are immediately incorporated in both the _staging_ and the _master_ branches. <!-- check how hotfixes are addressed: is there a need to create a v.2020.3.1 branch? If yes, update description. -->

![v2021.0](./img/v2021.0.png "v2021.1")



As mentioned above, this release schedule has been made to cover an annual cycle as an example, but this release schedule is intended to be established consistently over time.

# Release Delivery
Each release of the INSPIRE Reference Validator is fully managed and made available to the INSPIRE community through the folowing set of GitHub artifacts: 

* a **GitHub milestone**, named _v202x.y (dd/mm/yyyy)_ and published on the [Milestones section of the _community_ repository](https://github.com/inspire-eu-validation/community/milestones); the milestone lists the issues whose solutions are included in the current release;

* a **GitHub release**, named _v202x.y (dd/mm/yyyy)_ and published on the [Release section of the _community_ repository](https://github.com/inspire-eu-validation/community/releases). The release notes include:
  * a list of new features to the ATS, ETS and ETF
  * a list of bugfixes, each with the corresponding issue and pull request
  * a list of the enhancements, each with the corresponding issue and pull request
  * the new documentation produced, if any
  * assets, i.e. code packages required for deployment:
	  * _ets-repository-v202x.y.zip_, containing the _ets-repository_ repository corresponding to the release branch;
          * _etf-release-v202x.y.zip_, containing ETF deployment instructions and artifacts;
	  * _Source code.zip_ and _Source code.tar.gz_, including the content of the _community_ repository for the current release;
	  
* a **GitHub package**, published on the [Packages section of the _community_ repository](https://github.com/inspire-eu-validation/community/packages), including the instructions and resources needed to deploy the current release of the INSPIRE Reference Validator through the use of Docker.

* update of the **[GitHub issue tracker of the _community_ repository](https://github.com/inspire-eu-validation/community/issues)** by changing the label of the issues solved within the current release from _solved_ to _deployed in reference validator_ and by closing them;

* update of the **[Validator issues project board](https://github.com/inspire-eu-validation/community/projects/1)** by moving all the issues labeled as _deployed in reference validator_ to the column _Production: latest release_.
