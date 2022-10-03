# nanoHUB-Jupyter-template
This is a repository template for creating a nanoHUB Jupyter Notebook app.  The basic steps in the process are listed below. 

* Wherever you see `yourgithubaccount`, substitute the name of your GitHub account.  
* Wherever you see `yourgithubrepo`, substitute the name of your app's GitHub repo.  

These instructions assume that you already have a [nanoHUB account](https://nanohub.org/) and a [GitHub account](https://github.com/).

## 1) Create a GitHub repository for your new app using this template.
* Click the green "Use this template" button ![use_this_template](https://user-images.githubusercontent.com/35706811/193605808-f8e68353-bdf4-46ef-949d-4f3ea1f4c9ca.png) to start the process and open a page with several options to select and fields to fill in.

  ![GitHub_public_template](https://user-images.githubusercontent.com/35706811/193608966-c6ccad77-6af3-4031-9a8f-98b6246049d0.png)

* For Repository name, we suggest using your app's *shortname* to make life easier.  Refer to the documentation on registering a nanoHUB app for more information on the app short name. (link to come) 
* Write a short description of your app.
* Select whether the repo will be public or private. Public is easier.
* Do not check the box to include all branches.  nanoHUB only works with the master branch.
* Click the green button at the bottom to "Create repository from template".

Keep all of the folders and hidden files.  .keep files are present to force git to track initially empty directories. Should the directories become populated the .keep file can be removed.

## 2) Clone your app's GitHub repo into your personal nanoHUB filespace.
* Open a Jupyter Notebook session in nanoHUB and navigate to the directory into which you will clone your app's GitHub repo.
* In 2022, the latest Jupyter Notebook version is [Jupyter Notebook (202105) ](https://nanohub.org/tools/jupyter70). There are other versions that you can find by searching in the tools module in your nanoHUB dashboard.
* In your newly created GitHub repository, find the link you need by clicking the code download button and viewing the options.  
* In your nanoHUB Jupyter Notebook terminal, type `git clone https://github.com/yourgithubacount/yourgithubrepo`.


  ### 2a) If you set up a public GitHub repository:  
  * The repo should start cloning once you submit the git clone command.

  ### 2b) If you set up a private GitHub repository:
  * You will need to log in to your GitHub account. When prompted for your password, enter your [GitHub personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token).
      *  Use your GitHub account name and your personal token ....  You will not see the terminal respond when you paste in you token.  This is for security purposes. Hit return and you should see the repo starting to clone.
  * You will have to have an ssh key in nanoHUB and add the public key to your GitHub account to connect to your personal nanoHUB filespace. [Instructions for setting up an ssh key pair in nanoHUB](https://nanohub.org/kb/tools/sshkeypair).
  * Additionally, you need to invite nanohub-apps as a collaborator to your GitHub repo, in order to get the key to connect to nanoHUB/apps.
      * Click on the settings gear, then click on Collaborators.  Search for nanohub-apps, as shown in the following image:

      ![nanoHUB-apps_collaborator](https://user-images.githubusercontent.com/35706811/193604665-bee75798-3029-4a18-8df0-3777d166ea38.png)

## 3) Go to https://nanohub.org/tools/create to register and create your nanoHUB tool.
* In the section for Repository host, select "Host GIT repository on GitHUB".
* In the section for Git Repository URL, paste in the URL for your app's GitHub repo.
* For publishing option, select Jupyter notebook.

After you click the button to register your tool, you will be redirected to your tool's status page, and you will also receive an email with a link to the tool's project space in nanoFORGE.

Coming soon: a link to more complete instructions for building a Jupyter Notebook app.
