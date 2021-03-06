# Intro

In this tutorial we're going to work through a 'real life' example using git.

We'll be working with an example analysis workflow. My research is on cell free protein expression so I've provided some Fluoresence Timeseries data and plotting script in Python. The actual analysis is immaterial, if you wanted you could do the tutorial by editing a Microsoft Word Document.

To get a better understanding of how git might actually fit into a scientific workflow, we're going to:

* Download the script & data from Github to our computer
* Run the script to see what happens
* Edit that script
* Record the changes
* Upload the edited script back up to Github

And doing so learn not just how to use git but also some best practices to make the process as transparent and easy as possible.

# 1. Download the Materials

The first step is to download the materials from my remote Github repository.

To do this we use a git command called
`git clone`

How this command works is that it pulls the git repository from the given Github URL *& What else exactly?*, sets up remote?

## Set up project directory/folder on your own computer.

So to do this:

1. Create a new folder on your desktop and call it 'Example Git Timeseries analysis' or something. This will be the project folder into which you want to clone the git repo.

2. Next Open a Command Line Terminal (or Terminal if you're on Mac or Linux), and navigate to that newly created project folder.

  I have a tip for doing this which you may find useful:
    * Open the project folder in File Explorer/Finder and 'Copy Address as text' (*See Image*), then paste that address into the Command Line **within double quotes**. This will allow you to jump to the target directory in one step rather than tedious: `cd documents`, `cd labbook`, `cd myexperiments` navigation.

![navigation](https://github.com/aperkins19/Git_Guide_for_Scientists/blob/main/Assets/git3/effecient_navigation.png)


## Git Clone

Now that you have a folder to put your data and analysis scripts now it's time to grab the git repo and put it inside.

Ensuring that you're still navigated to the correct folder on your CLI run the `git clone` command. Now for this example we're going to grab a placeholder repo that I've made just for this example but you can use the same command by using any URL from Github that you like.

`git clone https://github.com/aperkins19/git_3_placeholder_project`

If it all goes well then you should see something line this:

![clone](https://github.com/aperkins19/Git_Guide_for_Scientists/blob/main/Assets/git3/clone_Example.png)

## Investigate our set up

So now that have cloned the repo, let's have a look around and see what's happened.

* Have a look at that folder in file explorer, you should see that all the files have been copied.
* Now using your CLI:

`git remote -v`

This allows us to see how the remote for the local git repo (which, as you will recall, was created by the git clone command) are wired up.
i.e. Which Github repositories it is configured to push and pull to. *n.b. You will likely never need them to be different.

Git Clone should have set them up for you and you should see that both point to:

`https://github.com/aperkins19/git_3_placeholder_project`






Git Commands

Setting your config MetaData (collaborator's know  you made the changes and how to contact you.)


`git --config --global user.name "Your Name"`

`git --config --global user.email "Your Email"`

`git config --global core.editor "nano -w"`


See your config settings:

`git config -l`

Initalise a git repo

`git init`

Look at your changes.

`git status`

What's in the directory?
Unix (mac):      `ls -al`
Bash (windows):     `dir`

If you've made a change to a file (e.g. myscript.py) git will see that

`git status`

But at this stage you haven't told git to record the changes. Add the file to the stage with:

`git add myscript.py`

When you call git status now, that file will be staged. You can add all the files whose changes you want to record with 'add'.

Once you've added all the changed-files to the stage that you want, you can record the changes all in one go with :

`git commit -m "Notes talking about why you made the changes, what you did etc."`

Exercise:
1. Make some changes! E.G. "nano mars.txt" to add lines, or you could create a new file.
2. Add changes to git. E.G. "git add mars.txt"
3. Commit those changes, E.G. "git commit",  with informative errors.
4. Look around with "git status", "ls", "git log", etc.

##########################################

This might be helpful for some :)
It's a GUI software for visually looking at your git commits/versions/branches in a project.

https://www.sourcetreeapp.com/

https://www.hostinger.com/tutorials/best-git-gui-clients/



 ################################################

 SOLUTION FOR AUTHENTICATING YOUR GIT ACCESS USING WINDOWS.

 https://www.youtube.com/watch?v=JCcrdW4Llm0







# Gittyfying a project folder i.e. initalising a local git repository
