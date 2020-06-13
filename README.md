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
git config -- global user.name = 'Muhammed'
```
7) To set an email to configuration email
```shellscript
git config -- global user.name = 'muhammedbuyukkinaci@gmail.com'
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
git rm -r --cached
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
40) To clone a Remote Repository to The Local Repository
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
45) Fetches a specific branch, from the repo. Leave off branch to fetch all remote refs.
```shellscript
git fetch <remote> <branch>
```
46) To fetch the specified remote’s copy of current branch and immediately merge it into the local copy.
```shellscript
git pull <remote>
```
47)To push the branch to remote, along with necessary commits and objects. Creates named branch in the remote repo if it doesn’t exist.
```shellscript
git push
<remote> <branch>
```
48 ) To Reset staging area to match most recent commit, but leave the working directory unchanged.
```shellscript
git reset
```
49 ) Reset staging area and working directory to match most recent commit and overwrites all changes in the working directory.
```shellscript
git reset --hard
```
50 ) Reset staging area and working directory to match most recent commit and overwrites all changes in the working directory.
```shellscript
git reset <commit>
```
51 ) Reset staging area and working directory to match most recent commit and overwrites all changes in the working directory.
```shellscript
git reset --hard <commit>
```
52)To Fetch the remote’s copy of current branch and rebases it into the local copy. Uses git rebase instead of merge to integrate the branches.
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
