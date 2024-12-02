Thank you for wanting to contribute to the Open Data Set Repository. This repository relies on user edits and submissions in order to stay up to date and expand itself to serve as many users as possible. The following steps will help you both create a new guide or make an edit to an existing guide.

## Step 1 - Creating a New Branch
Whether you are editing an existing guide or creating a new one the first step is to create a new branch from main in order to work on your new changes. Name the branch according to the changes you are proposing. If you are fixing an existing guide, name the branch "fix/{name of guide}". If you are making a new one, use the format "new/{name of guide}"

In order to create a new branch first navigate to the github repository either using the button in the site header or by navigating to [link](https://github.com/opendatasets1/UMD-OpenDataset). Once you are on the site, click on the dropdown by the name of the branch and type in the name of your branch, as shown in the image below.
![New Branch Image](./__img/Screenshot%202024-12-02%20at%2010.36.38 AM.png)

Click on the create branch button in order to create the new branch.

## Step 2 - Drafting the Edit file
If you are editing an existing guide check the 'User Guide Editing' folder for a .docx file to see if an editable version of the particular user guide exsits. Although, beware that the editable doc may not be up to date with the current guide. Reference the current guide to see the most up to date revision. If a .docx file does not exist for the guide you want to edit, download the pdf locally from the website, and edit it as a word document.

If you are starting a new guide, write the initial draft using word or google docs on your personal device. If you need a starting point for how to format the user guide reference [this template](./New%20Guide%20Template.md) or previous user guides for how to format your guide.

Once you are done writing your initial draft, and or making any changes. Upload the file to the editing folder within the branch that you have create. This can be done by clicking into the 'User Guide Editing' folder in git and hitting the 'Add File' button in the top right as can be seen in the image below.
![Upload Image](./__img/Screenshot%202024-12-02%20at%2010.52.23 AM.png)

After clicking on the upload image button you will be redirected to a page where you can drag and drop your word or google document. Add a commit message saying that you are uploading the guide, like below, and commit the changes.
![Commit Changes](./__img/Screenshot%202024-12-02%20at%2010.55.45 AM.png)

## Step 3 - Reviewing Changes
Once you have uploaded the initial draft of the user guide alert the repository owner (currently Mary Ann Francis, mfranci1@umd.edu), by emailing their UMD email. If you are updating a guide, use the subject, "Open Dataset Repository - Guide Update for {guide name}". If you are proposing a new guide, use "Open Dataset Repository - New Guide Proposal". In the email, include a link to your uploaded file in the new branch as well as details regarding what you have added to the repository.

Based on any changes requested by the repository owner, add those edits to the file, and then re-do steps 2 and 3 until approved.

**DO NOT MOVE ON TO THE STEP 4 BEFORE GETTING APPROVED BY THE REPOSITORY OWNER**

## Step 4 - Finalizing Changes and Editing the Website
Congratulations on getting your change approved. Now it is time to productionize the change for the main website. Now that you have had your guide approved, export it as a pdf, and make sure that the formatting is correct and doesn't have any issues. Next, still in your created branch, go to the 'Current User Guides" folder and upload the PDF using the same method used in Step 2. If you are adding a brand new guide, just upload the new PDF. If you are updating an existing guide, delete the existing pdf, and upload this new one. Don't worry about making any breaking changes, git automatically does version controlling which allows reverting any changes if needed.

Once you have uploaded this new guide it is time to add a link to that in the main page of the site. Go to your new branch in Github and click on the 'index.md' file. Once you click on this file hit the edit button in the top right corner as shown below.
![Edit Index.md File](./__img/Screenshot%202024-12-02%20at%2011.14.11 AM.png)

Once you hit the edit button a text editor will pop up with the file. If you are adding a new user guide, and another bullet point to the table and add a title to your guide as well as the link to it as shown below. 
![Add New Line](./__img/Screenshot%202024-12-02%20at%2011.17.14 AM.png)

The link to the file should always be in brackets. The link should start with `./Current%20User%20Guides/` and then have the name of your pdf file. Replace any spaces with `%20`.

If you are replacing an existing guide instead of adding a new one, you shouldn't have to complete this step unless you change the name of the pdf. While this is not recommended, if the pdf name is changed, update the link to reflect that change. Once you are done, hit the commit changes button as shown above and commit any changes.

## Step 5 - Merging Changes
Once all changes have been committed and have been reviewed. It is time to create a pull request and merge the changes to the main branch. Go to the repository page and click on the "Pull Requests" tab in the navigation bar as shown below.
![Pull Request Tab](./__img/Screenshot%202024-12-02%20at%2011.28.42 AM.png)

After navigating to this tab click on the 'New Pull Request Button' to start a new pull request. Once you have clicked on this choose the correct branches as the target and the source branches as shown below. The base should be the main branch and the compare should be the branch you have created. 
![New Pull Request](./__img/Screenshot%202024-12-02%20at%2011.35.38 AM.png)

Now hit "Create Pull Request" to start a new pull request. Once you create a new pull request it will start to look at the changes and see if there are any conflicts. If any conflicts arise, resolve them before you are able to merge. Once all conflicts have been resolved, the project will automatically add the Code Owner as the reviewer. They will be notified of the pull request automatically, but also send them an email (the code reviewer was linked in step 3), to let them know you have started a pull request. They will review the changes and approve the request if everything looks good. Once the request has been approved, it will allow you to click merge at the bottom of the page. Once this merge is complete it will kick off the deployment process. The deployment process usually takes 5-10 minutes after which your changes should be visible in the original site.


