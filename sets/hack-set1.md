#Hack Set #1
###Create Repo
```bash
mkdir repo
cd repo
git init
ls -l
ls -la
tree .git
```

###Create a file
```bash
vi foo
git add foo
git commit
```

###Edit foo
```bash
git add foo
git commit
```

###Create New Branch `feature`
```bash
git branch feature
git checkout feature
```

###Add New File to `feature`
```bash
emacs bar
git add bar
git commit
```

###Merge
```bash
git checkout master
git merge
git log --decorate --graph --stat
```

###New Feature -- Recursive Merge
```bash
git checkout feature
echo "fixed the bar" >> bar
git add bar
git commit -m "bar bug fix"

git checkout master
echo "also updating foo" >> foo
git add foo
git commit -m "another sna foo"

git merge foo

git log --decorate --graph --all
```

