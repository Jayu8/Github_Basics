Configuring remote github account in local - One time
```
git config --global user.email "123"
git config --global user.email 123@outlook.com
```

Start
```
git clone <link>
git remote set-url origin <link>
```
Pulling and adding stuff into local from remote
```
git pull origin master
git add <filename>    (git add . for all)
git status
git commit -am "Description"
git status
git push origin master 
```


Forked Repositories 
```
git fetch --all
git remote add upstream git://github.com/ORIGINAL-DEV-USERNAME/REPO-YOU-FORKED-FROM.git
git fetch upstream
git pull upstream master
git push origin master
```
You can't merge with local modifications. Git protects you from losing potentially important changes.

You have three options.
1. Commit the change using
```
    git commit -m "My message"
```
2. Stash it.

Stashing acts as a stack, where you can push changes, and you pop them in reverse order.

To stash type:
```
git stash
```
Do the merge, and then pull the stash:
```
git stash pop
```
3. Discard the local changes
```
git reset --hard. or git checkout -t -f remote/branch
```
3. a) Discard local changes for a specific file
```
git checkout filename
```
