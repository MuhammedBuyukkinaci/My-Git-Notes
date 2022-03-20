# My-Git-Notes

1) Software Development is a continuous process

2) We are required to get snapshots of our software

3) Why do we use Git?

- To follow development processes

- To collaborate

- Enabling us to split our project into particular branches

4) Illustration of Working Directory, Staging Area, Local Repository, Remote Repository

![alt text](https://miro.medium.com/max/3834/1*g-iW9rUZVeHSdKNnVbAuQg.png)

5) To see the properties of git configuration
```shellscript
git config --list
```
6) To set a name to configuration name
```shellscript
git config --global user.name "Muhammed Buyukkinaci"
```
7) To set an email to configuration email
```shellscript
git config --global user.email 'your_email_address@gmail.com'
```
8) To create a local repo
```shellscript
git init
```
9) To get information about files and changes
```shellscript
git status
```
10) To transfer all FILES to staging area
```shellscript
git add .
```
11) To transfer staged changes to The local repository
```shellscript
git commit -m "Transfering to the local repository"
```
12) An VSCode extension named as Live Server can be used in HTML

13) To send all CHANGES to Staging Area
```shellscript
git add -A
```
14) After renaming a file, add all files to The Local Repository
```shellscript
git add .
```
15) To see short version of changes:
```shellscript
git status -s
```

16) While committing, messages can be copies of the results of 'git status'


17) To roll back a change from Staging Area:
```shellscript
git restore --staged filename
```
18) To roll back a change from Working Directory
```shellscript
git restore filename
```
19) To see latest commit
```shellscript
git show
```
20) To see all commits in The Local Repository
```shellscript
git log
```
21) To see summary of commits
```shellscript
git log --online
```
22) To see only latest 2 commits
```shellscript
git log -p -2
```
23) To see commits after a time period
```shellscript
git log --since=10minutes
```
24) To go back to a specific commit
```shellscript
git checkout 7_DIGIT
```
25) To go forward to latest commit
```shellscript
git checkout master
```

26) Checkout can be used to go back to previous versions.


27) To delete a commit and its effects
```shellscript
git revert 7_DIGIT
```
28) To revert a change of revert
```shellscript
git revert 7_DIGIT
```

29) While using ```git reset```, take care a lot. To remove staged files from Staging Area(Not Working Directory)
```shellscript
git reset FILE_NAME
```
30) To roll back from only The Local Repository
```shellscript
git reset --soft HASH_NUMBER
```
31) To roll back from Staging Area and The Local Repository
```shellscript
git reset --mixed HASH_NUMBER
```
32) To roll back from  Working Directory, Staging Area and The Local Repository
```shellscript
git reset --hard HASH_NUMBER
```
33) Put the names of files that you don't want to be tracked into .gitignore file. A sample .gitignore file was listed below.
```
log.txt
directory/
*.py
```
34) Create .gitignore firstly while creating a project. If you didn't do this, clear cache by command below.
```shellscript
git rm -r --cached .
```
![alt text](https://i2.wp.com/digitalvarys.com/wp-content/uploads/2019/06/GIT-Branchand-its-Operations.png?resize=1024%2C563&ssl=1)

35) To create a new branch
```shellscript
git branch branch_name1
```
36) To list all branches in a project
```shellscript
git branch -a
```
37) To pass to a different branch
```shellscript
git checkout branch_name1
```
38) To pass back to master branch
```shellscript
git checkout master
```
39) While on master, merge different branches into master.
```shellscript
git merge branch_name1 branch_name2
```
40) To clone a Remote Repository to The Local Repository. While cloning, a default .git directory is created.
```shellscript
git clone REMOTE_REPO_NAME
```
41) To show which files to be removed from working directory
```shellscript
git clean -n
```
42) To clean out which files to be removed from working directory
```shellscript
git clean -f
```
43) Rebase the current branch onto base. base can be a commit ID,branch name, a tag, or a relative reference to HEAD.
```shellscript
git rebase <base>
```
44) To add a new remote to local repo
```shellscript
git remote add origin https://github.com/user/repo.git
```
45) To fetch a specific branch from the remote. Leave off branch to fetch all remote refs. It allows only copying, not merging
```shellscript
git fetch <remote> <branch>
```
46) To fetch the specified remote’s copy of current branch and immediately merge it into the local copy. git pull = git fetch + git merge
```shellscript
git pull <remote>
```
47)To push the branch to remote, along with necessary commits and objects. Creates named branch in the remote repo if it doesn’t exist.
```shellscript
git push
<remote> <branch>
```
48) To Reset staging area to match most recent commit, but leave the working directory unchanged.
```shellscript
git reset
```
49) Reset staging area and working directory to match most recent commit and overwrites all changes in the working directory.
```shellscript
git reset --hard
```
50) Reset staging area and working directory to match most recent commit and overwrites all changes in the working directory.
```shellscript
git reset <commit>
```
51) Reset staging area and working directory to match most recent commit and overwrites all changes in the working directory.
```shellscript
git reset --hard <commit>
```
52) To Fetch the remote’s copy of current branch and rebases it into the local copy. Uses git rebase instead of merge to integrate the branches.
```shellscript
git pull --rebase <remote>
```
53) To Forces the git push even if it results in a non-fast-forward merge. Do not use the --force flag unless you’re absolutely sure you know what you’re doing.
```shellscript
git push <remote> --force
```
54) To push all of your local branches to the specified remote.
```shellscript
git push <remote> --all
```
55) Tags aren’t automatically pushed when you push a branch or use the --all flag. The --tags flag sends all of your local tags to the remote repo.
```shellscript
git push <remote> --tags
```
56) To Show difference between working directory and last commit.
```shellscript
git diff HEAD
```
57) To show difference between staged changes and last commit
```shellscript
git diff --cached
```

58) To delete a branch
```shellscript
git branch -d branch_name1
```

59) To add a new developer to the existing project on GitHub, Settings --> Manage Access --> Invite a collaborator

60) github.com/octocat/Spoon-Knife project can be used while forking a project. After forking a project and making changes, we should create a pull request. Our pull request is going to be evaluated by project owner or team leader.

61) We can use GitHub to host our static websites. Make a repository named as GITHUB_USER_NAME.github.io .

62) To show which repos are available on remote

```shellscript
git remote -v
```

# Sources

- https://www.youtube.com/watch?v=SX8bHqXt8ws
- https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet


63) How to git restore a particular extension

```
git checkout -- "*.xml"
```

64) How to add a new remote repository to a local repository

```shell
#origin is the name of a remote repository in local computer.
git remote add my_awesome_new_remote_repo git@github.com:MuhammedBuyukkinaci/My-Git-Notes.git
git remote add origin git@github.com:MuhammedBuyukkinaci/My-Git-Notes.git
```

65) To remove a remote repository from a local repository

```
git remote remove NAME_OF_REMOTE_REPO_IN_LOCAL
# Example:
git remote remove origin
```

# Git For Professionals

### Perferct Commit

66) [git-tower.com](https://git-tower.com) is a GUI to improve git facilities.

67) Git staging area is enabling us to make 2 different commits from a single file

```file1.py

import os # go to commit 1

import sys # go to commit 2

```

68) Changes in a topic should belong to a single topic/issue.

69) `git add -p index.html` is  chooging parts of a file to a commit, not a whole file. We are prompted to choose which parts to be committed thanks to `-p` flag.

70) `git commit` has a subject and a body section. After putting changes to a staging area, type `git commit` and a window is prompted. The first line is commit subject that shouldn't exceed 80 characters.The second line is empty. The third line is the detailed explanation

`
### Branches

71) 3 types of branches:
 
- Mainline branches like main or master, long living
- Integration branches like develop or staging, long living
- Feature branches (refactoring, experiment, bugfix, release etc.), short running

![Video Link](https://github.com/MuhammedBuyukkinaci/My-Git-Notes/blob/master/images/001.jpeg)

72) If you have staging, development, production environments, it is advised to mirror branches (main, develop etc.)

73) Commits shouldn't be directly merged/rebased to integration and mainline branches. They should be committed on feature branches.

74) Short lived branches are created for certain purposes like bugfix or refactoring or experiments or feature adding.

75) Githubflow is advocating a simple approach. 1 long running branch + feature branches(feature, bugfix, refactoring).

![Video Link](https://github.com/MuhammedBuyukkinaci/My-Git-Notes/blob/master/images/002.jpeg)


76) Gitflow is a more structured approach.

- main: current production code
- develop: feature branches start from develop branches and merged back on develop branch
- feature: new attributes or bugfixes or refactoring are coded on feature branches.

![Video Link](https://github.com/MuhammedBuyukkinaci/My-Git-Notes/blob/master/images/003.jpeg)


77) A tag named release should be added to release branches

### Pull Requests

78) Pull Request is a feature of git hosting platforms (github, bitbucket, gitlab)

79) Pull Request invites others(reviewers) to give feedback before merging changes in code.

80) Pull Request is enabling us to improve an open source project on a hosting platform like github. This happens in the following way:

Fork      --> Change (Improve) the forked repo --> Open a pull request to original repo from new
the repo      on a new branch                      branch of forked repo to master branch of original repo

81) Pull Requests are always based on branches not on individual commits.


### Merge Conflicts

82) `git merge`, `git rebase`, `git pull`, `git cherry-pick`, `git stash apply`, all of these may result to a merge conflict.

83) Merging branches works effortlessly in most of the times because git is usually able to figure out what is going on.

84) Contradictory changes like `same line changed by 2 different branches, a file modified on 1 branch and deleted in other etc.` may result in merge conflicts.

85) You can't ignore merge conflict. You have to deal with before you can continue your work. Dealing with a merge conflict doesn't mean you have to resolve it; you can undo it and this is sometimes really helpful.

```
git merge --abort

git rebase --abort
```

86) git is marking the promlematic ares via *>>>>>* or *<<<<<<<*. *======* is separating changes of different commits

![Video Link](https://github.com/MuhammedBuyukkinaci/My-Git-Notes/blob/master/images/004.png)

87) The solution to merge conflicts is to clean up the file. GUI options like git-tower and Github Desktop are really helpful on solving merge conflicts. On the other hand, there are dedicated merge tools. For complicated conflicts,it is great to have  dedicated merge tool at hand. A merge conflict tool can be configured via `git config`.

88) After dealing with merge conflict via GUI or manually or git merge tool, We have to commit this situation like any other ordinary change.







