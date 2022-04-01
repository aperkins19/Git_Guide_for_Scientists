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

##########################################

How to fix github permissions and set up access:
 https://docs.github.com/en/get-started/quickstart/set-up-git
 
 
 Links to more resources on git and github:
 https://carpentries-incubator.github.io/good-enough-practices/06-track_changes/index.html#some-git-resources
 
 
 ################################################
 
 SOLUTION FOR AUTHENTICATING YOUR GIT ACCESS USING WINDOWS.
 
 https://www.youtube.com/watch?v=JCcrdW4Llm0
 
 ###############################################
 
 
 
 ## Evaluation day 2 (git with hasty improvisation)

Please list 1 thing you liked or found particularly useful
-I learnt what git is and how you can link up to git hub
-Learned about what git and github are using for
-learnt about github which I hope could be helpful .
-
-



Please list another think you found less useful, or that could be improved
-A follow up lesson would be useful 
-
-
-
