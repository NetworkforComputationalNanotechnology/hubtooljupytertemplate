# nanoHUB-Jupyter-template
This is a repository template for creating a nanoHUB Jupyter tool.

Keep all of the folders and hidden files.  
.keep files are present to force git to track initially empty directories.
Should the directories become populated the .keep file can be removed.
Your Jupyter notebook files will go in the top level directory.  More information will be available in nanoFORGE once you register your new tool.

1) Click the green "Use this template" button to create a copy of this repository in your own GitHub account.
* Type in the name of your repository. You can use your tool short name, or something related to your tool's name, to make life easier.
* Select whether the repo will be public or private. Public is easier.
* Click the green button at the bottom to "create repository from template".

2) Go to your newly created repository and copy the link to clone the repo to nanoHUB (click the code download button).

2a) If you set up a public repository, you will use the public https:// link to set up the connection with nanoHUB.
* Click the clipboard icon to copy the URL to the clipboard.

2b) If you set up a private repository, there are more steps:
* You will have to have an ssh key in nanoHUB and add the public key to your GitHub account.  Intructions are here: https://nanohub.org/kb/tools/sshkeypair.
* You will use the private ssh:// link to set up the connection with nanoHUB.
* You need to invite nanohub-apps as a collaborator to your repo, in order to get the key to connect to nanoHUB.

3) Go to https://nanohub.org/tools/create to set up and register your nanoHUB tool.
* In the section for Repository host, select "Host GIT repository on GitHUB".
* In the section for Git Repository URL, paste in the link copied to the clipboard.
* For publishing option, select Jupyter notebook.

After you click the button to register your tool, you will be redirected to your tool's status page, and you will also receive an email with a link to the tool's project space in nanoFORGE.

[Include a link here to more complete instructions for building a Jupyter Notebook Tool.]

For a Jupyter notebook tool, put your notebooks and associated files in the top level directory. Keep all of the additional, unused folders and files - just ignore most of them. You will need to update the invoke script in the middleware folder.
