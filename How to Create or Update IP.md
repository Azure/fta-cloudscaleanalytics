# How to Create or Update IP

This article outlines the steps needed to create or update existing FTA IP. It does not cover how to create or update the official Microsoft documentation.

## Step 1: Inform the Category Leads
1. Reach out to the category leads for the FTA scenario in question.  You may find the list of category leads here [FTA Service Leads](https://microsoft.sharepoint.com/teams/fasttrackforazure/PM/FastTrack%20for%20Azure%20PMO/Service%20Team%20Engagement%20&%20PG%20Contacts/Service%20Team%20Engagement/FTA%20Service%20Leads_Nov2018.xlsx)
2. Let them know which IP you intend to create. This is to ensure we avoid duplication of efforts as well as to ensure the team is aware of what IP is coming in the pipeline.


## Step 2: Prepare your Remote Git Environment: Create a Remote Branch

Note: Some teams utilize the work in progress repository: [FTA WIP Repository](https://github.com/Azure/fta-wip). We will only utilize this repository to create new IP if a new scenario is being added entirely. This is not a common case, so we will not document it here.

1. Open a new browser and navigate to https://github.com/Azure/fta-deliveryhowto.
2. Create a new remote branch. Click on the "__Branch: master__" dropdown button. Type in a new branch name.

> Branch name should include your alias: **_youralias/fta_scenario_name_**

![Image](/img/Github.newbranch.png?raw=true)

3. Click on the "Create branch __branchname__ from master" popup button.


## Step 3: Prepare your Local Git Environment: Create a Local Branch
1. Download and install Git.exe from https://git-scm.com/downloads. Choose defaults, and choose to update the PATH variable:

![Image](/img/installgit.png?raw=true)

2. Open __Git CMD__ to open the Git command line.
2. Create and navigate to a local repository folder.

> md c:\sourcerepo

> cd c:\sourcerepo

2. Clone the newly created remote branch to your machine

> c:\sourcerepo>git clone https://github.com/Azure/fta-deliveryhowto --branch __fanyv/intelligent-apps__

![Image](/img/gitclone.png?raw=true)

3. This will automatically create a new directory with the contents of the repository (fta-deliveryhowto). Navigate to the newly created directory.

> c:\sourcerepo>cd fta-deliveryhowto

4.  Verify you have downloaded the correct branch

> c:\sourcerepo\fta-deliveryhowto>git status

![Image](/img/gitstatus.png?raw=true)


## Step 4: Make Changes on Local branch and Merge Changes into Your Remote Branch
1. Create new files or make modifications to existing files on your local machine. If you are new to markdown files, recommend you review the following tutorial: https://guides.github.com/features/mastering-markdown/. You can use VSCODE to edit markdown files (https://code.visualstudio.com/Docs/languages/markdown).
2. When you are done making your changes. Commit your changes to your local branch

> c:\sourcerepo\fta-deliveryhowto>git commit -a -m "Created Cognitive Services IP."

3. Push changes from your 

Create a pull request.
*  Add reviewers to your pull request. You should add the service leads as reviewers.
* Email any additional reviewers from the v-team

>Question: Why not just add other non-category leads directly as reviewers in the pull request? Avoid additional step of emailing them

* Be sure to choose the option to delete the branch immediately after the pull request is accepted.

2. The changes will be merged into the master branch after the reviewers accept your changes.





