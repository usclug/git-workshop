##Git Configuration
###Git Variables
```bash
git config --global user.name "Tommy Trojan"
git config --global user.email "ttrojan@usc.edu"
git config --global color.ui auto
git config --global core.editor vi
git config --global merge.tool vimdiff
git config --global core.autocrlf input
```

###SSH Key Pair
```bash
ls -l ~/.ssh
ssh-keygen -t rsa -b 2048 -C "ttrojan@usc.edu"
cat ~/.ssh/id_rsa.pub
```

