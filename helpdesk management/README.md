# Introduction
The establishment of a proper communication with the INSPIRE Validation community is a key asset for the operation, maintenance and update of the INSPIRE Reference Validator. The [helpdesk of the INSPIRE Reference Validator](https://github.com/inspire-eu-validation/community/issues) is the core of the communication strategy, since it is the platform where users can report bugs, propose new features and start discussions on the Validator. The objective of this document is to illustrate the systematic workflow setup by the INSPIRE Validation team to address and manage the issues reported by users in the Validator helpdesk.

<!-- For this, the issue management functionalities offered by GitHub are being used, providing assistance to the users' requests, as well as offering detailed information of the changes and hotfixes that will be included in the different versions.
In this way, a workflow is established for the Helpdesk Management that allows to carry out in a systematic and organized way the management of the different issues that are incorporated to the Community repository.
So, the aim of this document is to explain in detail the procedure established for the issues management in order to have a proper understanding in the defined process for its management. -->

# Helpdesk management workflow
The helpdesk management workflow defines and organizes the set of actions performed by the INSPIRE Validation team as well as those expected from the users of the INSPIRE Validator. The workflow makes use of a number of GitHub artifacts: labels, milestones and the project board.

## GitHub labels <!-- could be removed, if not needed -->
To be able to know the status of each issue reported in the helpdesk (from the initial assessment to the final implementation of a solution for it), a number of labels are used. These are included on [this page](https://github.com/inspire-eu-validation/community/labels) and are described in more detail below in the chronological order in which they are used while managing each Validator issue:

* **_under analysis_**: this label is assigned after the issue has been opened, and indicates that the INSPIRE Validation Team is performing a first analysis to figure out what is the problem and how to address it; in case additional information is needed, the INSPIRE Validation Team asks the user to provide it directly in the issue discussion.
* **_discussion_**: this label is assigned to the issue, in case the initial analysis reveals that it is neither a bug of the INSPIRE Reference Validator nor a new requested feature; in other words, the issue will remain open for community discussion but no further action will be made by the INSPIRE Validation Team;
* **_under development_**: in case the initial analysis reveals that a change in the INSPIRE Reference Validator is needed, this label is assigned to the issue to indicate that the INSPIRE Validation team is developing a solution for the problem reported;
* **_ready for testing_**: this label is assigned to the issue, to indicate that a solution for the problem reported has been developed by the INSPIRE Validation team and is ready to be tested in the [Staging instance](http://staging-inspire-validator.eu-west-1.elasticbeanstalk.com/etf-webapp/) of the INSPIRE Reference Validator; in the issue discussion, the user who originally reported the problem is invited to test the solution and provide feedback;
* **_solved_**: this label is assigned to the issue after the user has tested the developed solution in the [Staging instance](http://staging-inspire-validator.eu-west-1.elasticbeanstalk.com/etf-webapp/) of the INSPIRE Reference Validator and has confirmed that it actually solved the problem in the issue discussion; no issue is marked as _solved_ without such a written confirmation from the user.
* **_deployed in reference validator_**: this label is assigned to the issue, when the developed solution is also included in the [Production instance](https://inspire.ec.europa.eu/validator/) of the INSPIRE Reference Validator; the release schedule of the Production instance is described [here](https://github.com/inspire-eu-validation/community/tree/master/release%20strategy). Once the solution has been included in the Production instance, the issue is finally closed.

The diagram below shows the full helpdesk management cycle for each issue. The two swim lanes clearly identify the actions expected by the use 

Below is a diagram describing the workflow of an issue, along with the states in which it can be found and which actor takes action on it.

![Helpdesk Management Workflow](./img/HelpdeskWorkflowPublic.png "Helpdesk Management Workflow")

In the diagram above, the workflow is triggered by the submission of an issue in GitHub by a community user.

In the first instance, the Validation Team contacts the user and sets a tag "under analysis" to proceed to collect the necessary information to solve the issue. At this point, it is possible to iterate with the user to request more detail about the submitted issue.

Once there is enough information, the issue is classified either as "discussion", in case it is not an issue directly related to the Validator or it is related with a new feature request, or as "under development", so the tasks associated to its resolution are carried out.

After the development of the tasks for the resolution of the issue and its integration in the INSPIRE Reference Validator Staging environment, the issue is marked as "ready for testing". At this stage, the explicit validation of the user is requested to ensure that the resolution of the issue provides, in fact, enough coverage to the needs initially requested. 

If the resolution of the issue covers the needs raised, it is incorporated into the INSPIRE Reference Validator roadmap and, once this issue is deployed in the production environment, the issue is marked as "closed". Otherwise, the workflow may go back in order to iterate until the issue is finally closed.

In this way, the workflow for attending to incidents related to the INSPIRE Reference Validator is completed.


<!-- In order to establish a proper issues management procedure, it has been created a workflow that allows to know at any moment the state of an issue. This workflow defines a set of actions for the resolution of issues in which both the users and the Validation Team will participate.
In this Helpdesk Management Workflow, issues go through a series of status that are marked by means of the use of labels that identify in a simple way the actions taken until the moment and the next actions to take.
In summary, the tags that an issue can be assigned with are the following:
* under analysis: indicates that the Validation Team is performing an analysis of the scope of the issue
* under development: shows that the Validation Team is running a development according to the analysis of the issue
* ready for testing: the development associated with the issue has been carried out and is available to the user for validation in the INSPIRE Reference Validator Staging environment
* solved: once the user has confirmed that the development carried out is adequate, the issue is marked as solved. Please note that only the issues of which the developed solution is accepted by the users will be incorporated to the next release in the Production environment
* closed: an issue is tagged as "closed" when it has been deployed in the INSPIRE Reference Validator environment
* discussion: if it is not an issue directly related with the INSPIRE Reference Validator or it is a new feature requested by an user, it is labeled for discussion -->
