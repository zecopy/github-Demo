# github-Demo

<h1>Basic operations of GIT :</h1>
<br>

1) CLONE : This creates a directory and downloads the remote repository existing on the github.(Copy of the repository actually)

2) INIT : This creates an empty git local directory, initialized with the git attributes.

3) PULL : This updates the change from the remote towards the local.

4) PUSH : This will update the changes of the local towards the remote.



<h1>Concepts of Branches :</h1>
Git works on the default branch called Main/Master. Several branches can be created on a single repository that will help to segregate the work of the project.
In order to update the content of one branch into another 'merge' operation  is performed.(i.e., copying the work of one branch into another)
In the local whatever changes we are doing are finally saved by using 'add' and 'commit'.(i.e., create,edit,delete all of them have to be saved with the help of 'commit' operation.)
<br>
NOTE: Repositories can either be PUBLIC or PRIVATE.
<br>


In order to start work in the local :<br>
-> Configure your registered email and the username.<br>
-> These configurations can be reset again for different userID's.<br>
-> $ git config --global user.name "my name"<br>
-> $ git config --global user.email "Someone@email.com"<br>
NOTE: Config is on two basis, Global & Local.<br>
-> $ git config --list<br>
-> $ git --version (current git version)<br>
-> $ git clone https://github.com/user.name/DemoProject.git<br>
-> .git folder(hidden) contains all configuration files.<br>
NOTE: Save is not the technical word in git, the technical word is commit.<br>
-> $ git add (file name) OR git add . (to add all the files) {Add command}<br>
-> $ git commit -m "Some message"<br>
-> $ git log {Provides the history of the commits} git log provides the history of the commit with the 'commit id' and 'commit msg'.<br>
-> $ git pull origin main<br>
-> $ git push origin main<br>


<h4>Command to create a local branch</h4>
-> $ git branch 'branchname'<br>
The new branch will be created from the parent branch. All the contents of the parent branch will be copied to the child branch.
After that they will behave as separate branches. The same operations can now be applied to the newly created branch.<br>
-> In order to switch to another branch the command is "$ git checkout BranchName"<br>
-> In order to rename the branch, the command is "$ git branch -m 'new branch name'"<br>
While creating the branches, only one folder will be created irrespective of the no. of branches.<br>


<h4>Deletion of branches from the local</h4>
-> $ git -d <Branch name>
<h4>Deletion of branches from remote</h4>
-> $ git push origin --delete <Branch Name>
<h4>Command to merge the branches</h4>
-> $ git merge <branch Name>
<br>
-> Git stash: The git stash command is used to temporarily save your uncommitted changes so you can work on something else (like switching branches) without losing or committing your work.The status is saved in the temporary reguster.<br>
-> $ Git status : This command provides the status on the the current working directory.<br>
-> Fork operation : It means to copy someone's work into your github account.<br>
-> merge + fetch = pull<br>
fetch  operation is capable of only reflecting  the changes from the remote. Pull operation reflects and updates the changes from the remote. When we use merge + fetch, this operation is equivalent to pull.<br>
-> when we want to publish the local project on the github, we will establish the connection by using the command '$ git remote add origin URL'.  
