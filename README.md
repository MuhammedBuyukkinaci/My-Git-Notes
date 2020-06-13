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

29) While using ```git reset```, take care a lot.


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
