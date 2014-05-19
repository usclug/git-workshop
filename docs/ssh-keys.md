#SSH Key-based Configuration

By default, git communicates with servers using the git protocol that works over [SSH](http://en.wikipedia.org/wiki/Secure_Shell). Therefore, it is advised to generate a set of [SSH keys](http://en.wikipedia.org/wiki/Secure_Shell#Key_management) for authentication purposes.

Here we will talk you through the process of generating SSH keys for your system.

As with [configuring git](git-config.md) the ssh key setup is performed manually through the command line. You would need to launch:

  + MacOS or Linux: Terminal
  + Windows: Git Bash

####Check Existing Keys
By default, SSH keys are stored in the `.ssh` directory of the user's home directory. The default file names are:
  + `id_rsa` &ndash; private key
  + `id_rsa.pub` &ndash; public key

If you have both files available, there is no need to create a new pair unless you want to overwrite the current pair you have for security reasons.

To check if you have an existing pair:
```bash
#Check if you already have keys
ls -l ~/.ssh
```

#####Generate a New Key Pair

