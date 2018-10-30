```git
git clone git@github.com:YOUR-USERNAME/YOUR-FORKED-REPO.git
git remote add origin git@github.com:USERNAME/REPOSITORY-NAME.git
git clone https://github.com/paulboone/ticgit
git remote add https://github.com/paulboone/ticgit
```
```
git add -A   (force push introml)
```

```
git pull origin master
git add <filename>    (git add . for all)
git status
git commit -am "Description"
git status
git push origin master
```
git remove 
```
git rm filename
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
