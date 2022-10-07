# nanoHUB-Jupyter-template
This is a repository template for creating a Jupyter Notebook tool that you plan to publish in nanoHUB. The basic steps in the process are listed below. 

* Wherever you see `yourgithubaccount`, substitute the name of your GitHub account.  
* Wherever you see `yourgithubrepo`, substitute the name of your tool's GitHub repo.  

These instructions assume that you already have a [nanoHUB account](https://nanohub.org/) and a [GitHub account](https://github.com/).

## 1) Create a GitHub repository for your new tool using this template
* Click the green "Use this template" button ![use_this_template](https://user-images.githubusercontent.com/35706811/193605808-f8e68353-bdf4-46ef-949d-4f3ea1f4c9ca.png) to start the process. This opens a page that has several options for you to select and fields to fill in.

  ![GitHub_public_template](https://user-images.githubusercontent.com/35706811/193608966-c6ccad77-6af3-4031-9a8f-98b6246049d0.png)

* For **Repository name**, we suggest using your tool's *shortname* to make life easier.  Refer to the documentation on registering a nanoHUB tool for more information on the *shortname*. (link to come) 

* Select whether the repo will be **public** or **private**. 
     * nanoHUB encourages you to create a **public** GitHub repo. 
     * If you make your tools both open access in nanoHUB and open source in GitHub, this creates a greater potential for others to use, cite and build upon your work. 
     * Additionally, working with a public repo is technically much simpler and avoids periodic issues (such as firewalls) that can unexpectedly arise when working with a private repo.

* You do not need to check the box to include all branches. There is only one branch here, and nanoHUB only works with the main branch of your repo.

* Click the green button at the bottom to **Create repository from template**.

Keep all of the folders and hidden files.  .keep files are present to force git to track initially empty directories. Should the directories become populated the .keep file can be removed.

## 2) Clone your tool's GitHub repo into your personal nanoHUB filespace
It is convenient to work with separate windows or tabs to work with both your GitHub account and your nanoHUB account at the same time.
* Open a terminal in a Jupyter Notebook session in nanoHUB and navigate to the directory into which you will clone your tool's GitHub repo.
* In 2022, the latest Jupyter Notebook version is [Jupyter Notebook (202105)](https://nanohub.org/tools/jupyter70). There are also other versions that you can find by searching in the tools module in your nanoHUB dashboard.
* In your newly created GitHub repository, find the link to this repo by clicking the green code download button and viewing the options.  
  ![codeDownloadButton](https://user-images.githubusercontent.com/35706811/194592373-499642e4-7e61-4207-8608-d096aa064315.png)


### There are two ways to clone a repo: using HTTPS or using SSH  
If you use HTTPS, you will need to enter your credentials every time you push code to the repo.  By contrast, if you set up your accounts to use SSH, your credentials are stored in your accounts, and you don't have to enter them again as you work.
  
### To use the HTTPS URL:  
* Go to the HTTPS tab
* Click the clipboard icon to copy your tools's https URL to the clipboard.
* In your nanoHUB terminal, type `git clone` and then paste the URL from the clipboard and hit return.
* The full command will look like this: `git clone https://github.com/yourgithubaccount/yourgithubrepo`
* You will be prompted for your GitHub account name.
* You will be prompted for your GitHub password. Paste in your **GitHub Personal Access Token** and then hit return. You will not see any response from the terminal until you hit return.
  * [Instructions for creating a GitHub Personal Access Token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
* You should see the progress of your repo being cloned into nanoHUB. 

### To use the SSH URL: 
* You first have to have an ssh key pair in your nanoHUB account and add the public key to your GitHub account. 
  * [Instructions for setting up an ssh key pair in nanoHUB](https://nanohub.org/kb/tools/sshkeypair).
* Go to the SSH tab
* Click the clipboard icon to copy your tools's ssh URL to the clipboard.
* In your nanoHUB terminal, type `git clone` and then paste the URL from the clipboard. Hit return.
* The full command will look like this: `git clone git@github.com:yourgithubaccount/yourgithubrepo`
* You should see the progress of your repo being cloned into nanoHUB. 

## 3) Register your tool in nanoHUB
Go to https://nanohub.org/tools/create to register your nanoHUB tool.

* In the section for Repository host, select "Host GIT repository on GitHUB".

* In the section for Git Repository URL, type in the URL for your app's GitHub repo.
  * For a public GitHub repository, you can directly paste in the https URL from the clipboard: 
  
    `https://github.com/yourgithubaccount/yourgithubrepo`
  * For a private GitHub repository, you need to reformat the URL to have this form: 

    `ssh://git@github.com/yourgithubaccount/yourgithubrepo`

* For publishing option, select Jupyter notebook.

* If you set up a private GitHub repo, you also need to invite **nanohub-apps** as a collaborator in order to get the key to connect to nanoHUB/apps.
  * Click on the settings gear at the top of your repo, then click on Collaborators.  Search for nanohub-apps, as shown in the following image:

      ![nanoHUB-apps_collaborator](https://user-images.githubusercontent.com/35706811/193604665-bee75798-3029-4a18-8df0-3777d166ea38.png)


After you click the button to register your tool, you will be redirected to your tool's status page, and you will also receive an email with a link to the tool's project space in nanoFORGE.

Coming soon: a link to more complete instructions for building a Jupyter Notebook app.
