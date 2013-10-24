#Hack Set #2
##Remotes
```bash
cd ..
git clone --bare repo remote
tree remote
tree repo/.git

git clone remote work
cd work
git remote -v
```

##Bug fix branch
```bash
git checkout -b bugfix
echo "new bug fix" > buz
git add buz
git commit -m "a new bug fix"
```

##Push
```bash
git push origin
git push origin bugfix
```
