# How to Create or Update IP

This article outlines the steps needed to create or update existing FTA IP. It does not cover how to create or update the official Microsoft documentation.

## Step 1: Inform the Category Leads
Reach out to the category leads for the FTA scenario in question.  You may find the list of category leads here [FTA Service Leads](https://microsoft.sharepoint.com/teams/fasttrackforazure/PM/FastTrack%20for%20Azure%20PMO/Service%20Team%20Engagement%20&%20PG%20Contacts/Service%20Team%20Engagement/FTA%20Service%20Leads_Nov2018.xlsx)



## Step 2: Create IP Within a New Branch

Note: Some teams utilize the work in progress repository: [FTA WIP Repository](https://github.com/Azure/fta-wip). We will only utilize this repository to create new IP if a new scenario is being added entirely. This is not a common case.

1. Create a new branch. Specify a name for your branch.

> Sample branch name: **_youralias-fta-cloudscaleanalytics_**

2. Clone the branch to your machine
3. Create new files or make modifications to existing files on your local machine. You can use VSCODE to edit markdown files.
4. Git Commit changes

## Step 3: Merge Changes from Your Branch to the Master Branch
1. Create a pull request.
*  Add reviewers to your pull request. You should add the service leads as reviewers.
* Email any additional reviewers from the v-team

>Question: Why not just add other non-category leads directly as reviewers in the pull request? Avoid additional step of emailing them

* Be sure to choose the option to delete the branch immediately after the pull request is accepted.

2. The changes will be merged into the master branch after the reviewers accept your changes.





