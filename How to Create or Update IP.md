# How to Create or Update IP

This article outlines the steps needed to create or update existing FTA IP. It does not cover how to create or update the official Microsoft documentation.
<br>
<br>
<br>
<br>

## Step 1: Inform the Category Leads
1. Reach out to the category leads for the FTA scenario in question.  You may find the list of category leads here [FTA Service Leads](https://microsoft.sharepoint.com/teams/fasttrackforazure/PM/FastTrack%20for%20Azure%20PMO/Service%20Team%20Engagement%20&%20PG%20Contacts/Service%20Team%20Engagement/FTA%20Service%20Leads_Nov2018.xlsx)
2. Let them know which IP you intend to create. This is to ensure we avoid duplication of efforts as well as to ensure the team is aware of what IP is coming in the pipeline.
<br>
<br>
<br>
<br>

## Step 2: Prepare your Remote Git Environment: Create a Remote Branch

Note: Some teams utilize the work in progress repository: [FTA WIP Repository](https://github.com/Azure/fta-wip). We will only utilize this repository to create new IP if a new scenario is being added entirely. This is not a common case, so we will not document it here.

1. Open a new browser and navigate to https://github.com/Azure/fta-deliveryhowto.
2. Create a new remote branch. Click on the "__Branch: master__" dropdown button. Type in a new branch name.

> Branch name should include your alias: **_youralias/fta_scenario_name_**

![](/img/Github.newbranch.png?raw=true)

3. Click on the "Create branch __branchname__ from master" popup button.
<br>
<br>
<br>
<br>

## Step 3: Prepare your Local Git Environment: Create a Local Branch
1. Download and install Git.exe from https://git-scm.com/downloads. Choose defaults, and choose to update the PATH variable:

![Image](/img/installgit.png?raw=true)

2. Open __Git CMD__ to open the Git command line.
3. Create and navigate to a local repository folder.

> md c:\sourcerepo

> cd c:\sourcerepo

4. Clone the newly created remote branch to your machine

> c:\sourcerepo>git clone https://github.com/Azure/fta-deliveryhowto --branch __fanyv/intelligent-apps__

![Image](/img/gitclone.png?raw=true)

5. This will automatically create a new directory with the contents of the repository (fta-deliveryhowto). Navigate to the newly created directory.

> c:\sourcerepo>cd fta-deliveryhowto

6.  Verify you have downloaded the correct branch

> c:\sourcerepo\fta-deliveryhowto>git status

![Image](/img/gitstatus.png?raw=true)
<br>
<br>
<br>
<br>

## Step 4: Make Changes on Local branch and Push Changes into Your Remote Branch
1. Create new files or make modifications to existing files on your local machine. If you are new to markdown files, recommend you review the following tutorial: https://guides.github.com/features/mastering-markdown/. You can also use VSCODE to edit markdown files along with a convenient preview pane (https://code.visualstudio.com/Docs/languages/markdown).
2. When you are done making your changes. Commit your changes to your local branch. You must provide a short message describing the changes you are commiting.

> c:\sourcerepo\fta-deliveryhowto>git commit -a -m "Created Cognitive Services IP."

3. Push changes from your local repository into your remote repository.

If you have multiple local branches. Make sure you are on the correct local branch. You can run the git checkout command to switch to the correct local branch:

> c:\sourcerepo\fta-deliveryhowto>git checkout fanyv/intelligent-apps

Now, push your local branch changes to the remote branch:

> c:\sourcerepo\fta-deliveryhowto>git push origin fanyv/intelligent-apps

<br>
<br>
<br>
<br>

## Step 5: Create a Pull request to Request Changes be Merged into the Master Branch

1. Navigate to https://github.com/Azure/fta-deliveryhowto/pulls

2. Click on the __New pull request__ button.

![Image](/img/Github.newpullrequest.png?raw=true)

3. In the __Compare Changes__ screen, click on the __compare:master__ dropdown. Select your remote branch.

![Image](/img/Github.pullcompare.png?raw=true)

You should see a summary of changes to merge in the __Comparing changes__ screen.

![Image](/img/Github.pullcompare2.png?raw=true)

4.  Click on the __Create pull request__ button to proceed. In the __Open a pull request__ screen, enter a description. Click on the settings button next to Reviewers to add the scenario leads as reviewers.

    a. (Optional) Add any additional reviewers from the v-team to request they review and provide comments.

![Image](/img/Github.openpullrequest.png?raw=true)

![Image](/img/Github.openpullrequest2.png?raw=true)

5. Click on the __Create pull request__ button

6. The changes will be merged into the master branch after the scenario leads accept your changes.



## References
* Git Cheat Sheet https://services.github.com/on-demand/downloads/github-git-cheat-sheet/
* Git Reference https://git-scm.com/docs




