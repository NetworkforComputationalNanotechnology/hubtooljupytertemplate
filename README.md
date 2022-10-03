# nanoHUB-Jupyter-template
This is a repository template for creating a nanoHUB Jupyter app. The basic steps in the process are listed below.  For more background on using GitHub repository templates, see: https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template.

Keep all of the folders and hidden files.  
.keep files are present to force git to track initially empty directories.
Should the directories become populated the .keep file can be removed.
Your Jupyter notebook files will go in the top level directory.  More information will be available in nanoFORGE once you register your new tool.

1) Create a repository for your new app by copying this template in your GitHub account.
* Click the green "Use this template" button.
* Type in the name of your new app's repo. We suggest using your app's short name to make life easier.
* Select whether the repo will be public or private. Public is easier.
* Click the green button at the bottom to "create repository from template".

2) Clone your app's GitHub repo into your personal nanoHUB filespace.
* Open a Jupyter Notebook session in nanoHUB and navigate to the directory into which you will clone your app's GitHub repo.
* Go to your newly created GitHub repository and find the link copy to by clicking the code download button.  

2a) If you set up a public repository, you will use the public https URL to set up the connection with nanoHUB.  
* Click the clipboard icon to copy the URL to the clipboard
* Type `git clone https://github.com/yourgithubrepo` in your nanoHUB terminal (use your app's public https URL).

2b) If you set up a private repository, there are more steps:
* You need to invite nanohub-apps as a collaborator to your repo, in order to get the key to connect to nanoHUB/apps.
* You will have to have an ssh key in nanoHUB and add the public key to your GitHub account to connect to your personal nanoHUB filespace. Instructions are here: https://nanohub.org/kb/tools/sshkeypair.
* Type `git clone ssh://github.com/yourgithubrepo` to set up the connection with nanoHUB (use your app's private ssh URL).

After cloning your GitHub repo to your personal nanoHUB filespace, 

3) Go to https://nanohub.org/tools/create to set up and register your nanoHUB tool.
* In the section for Repository host, select "Host GIT repository on GitHUB".
* In the section for Git Repository URL, paste in the link copied to the clipboard.
* For publishing option, select Jupyter notebook.

After you click the button to register your tool, you will be redirected to your tool's status page, and you will also receive an email with a link to the tool's project space in nanoFORGE.

Coming soon: a link here to more complete instructions for building a Jupyter Notebook app.
