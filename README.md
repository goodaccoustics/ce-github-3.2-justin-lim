# ce-github-3.2-justin-lim

GitHub Authentication
1. SSH Key (commonly used together with git commands)
- Generate a SSH public and private key using ssh-keygen
- Store the private key into your local ssh file e.g ~/ssh/nameOfKeyFile
- Store the public key into GitHub
2. Using personal access token (commonly used for web transactions)
- Using a MFA app (e.g Google authentication) when verifying that you are the actual user issuing the command
3. Username and Password
- Using your username and password. However GitHub has increased security by requiring the use of a MFA app as a 2FA authentication.



***
Common GitHub commands


git init
- Create a new local git repository

git clone https://github.com/goodaccoustics/ce-github-3.2-justin-lim.git
- To clone the repository onto local machine after creating it on GitHub.com.
This should clone a main/master branch of the repository into your local machine.

git checkout -b "<<a new branch+name>>"
- To create a new branch separate from the main/master branch, so that any changes can go onto this branch first, instead of entering into the main/master branch

git pull
- If the local branch is out-dated from the remote branch, a git pull will pull down the latest changes of the remote branch into the local branch

git branch
- This command shows all the local branches of the repository downloaded into your local machine

git checkout <<an existing branch+name>>
- Assuming you have multiple branches on your local repository, this command enables you to switch to another branch

git status
- To check if there are any changes in the unstaged or staging area

git diff
- This command shows the changes between unstaged files and local repository files

git add . or git add <<filepath+filename>>
- To add the changes into the local repository's staging area

git commit -m "<<add a commit+message>>"
- To commit your changes into the local repository in preparation to push into the remote repository

git commit --amend
- Used when you want to change the commit message

git push origin <<branch_name>>
- To commit your changes into the branch in the remote repository

git log
- Tells you all the commits done on the existing branch. It tells which location your current branch is at now e.g HEAD -> main )
This will also expose out the commit IDs of each commit, allowing you to revert any changes that you have committed into the stage

git revert <<commit+Id>>
- This command allows to revert back any changes done in this commit ID
***

4 Most Commonly Used Git Commands
- git add <<file+ names>>
- git commit -m "commit message"
- git push origin <<branch+name>>
- git revert <<commit+id>>

Why? These commands represent a typical workflow required of a developer when saving down his work into the repository.