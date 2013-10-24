#Git Installation Instructions
This guide will assist you in installing git on your operating system of choice. You are advised to install git on all your machines. You will find below instructions for installing git on Linux, MacOS, Windows and aludra.

###Linux
Almost all major Linux distributions have git as a package that you can install using their standard package manager software.

  + Debian-based distro such as Ubuntu and Mint Linux use:
```bash
sudo apt-get install git
```

  + Fedora & CentOS can use:
```bash
sudo yum install git-core
```

####Test Your installation
To see if git was properly installed you should run the following command in a terminal window
```
git --version
```

The expected output for a successful installations is:
```
git version 1.8.4
```
Your version of git may be different, though.

###MacOS
There are multiple ways to install git on MacOS. The easiest way is to install the Apple pre-packaged version of git that comes with [Xcode](https://developer.apple.com/xcode/). The installation process is as follows:

  1. Install [Xcode](https://itunes.apple.com/us/app/xcode/id497799835) from the [Mac App Store](https://itunes.apple.com/us/app/xcode/id497799835)
  1. Install the **Command Line Tools** for Xcode using one of the following two methods:
    + Xcode &rarr; Preferences &rarr; Downloads &rarr; Components &rarr; Click `install` next to the Command Line Tootls; or
    + Download and install the Command Line Tools package from the [Apple Developers Downloads](https://developer.apple.com/downloads) page.


If you don't want to install Xcode, or just want to have a more recent version of git installed on your Mac. You can download and install the official [Mac package](http://git-scm.com/downloads) from the git website:
>http://git-scm.com/download/mac

_**Hint**_: In official Mac package, you will find alongside the git installer package a file called `setup git PATH for non-terminal programs.sh`. Make sure to run this script (by double clicking on it) after you install git.


####Test Your installation
To see if git was properly installed you should run the following command in a terminal window
```
git --version
```

The expected output for a successful installations is
```
git version 1.7.8
```

###Windows
Installing git on Windows is as easy as installing any other standard program. You start by downloading the [git Windows installer](http://git-scm.com/downloads):
>http://git-scm.com/download/win

Now, install the the package you just downloaded using the default settings for all the options.

Along with the git commandline tools, the package you just installed will install a Unix/Linux-like terminal named **Git Bash**. This application will allow you to access git and all the tools and commands needed to get you started.

####Test Your installation
To see if git was properly installed you should take the following steps:
  1. Start &rarr; Git &rarr; Git Bash
  1. In Git Bash, type `git --version`

The expected output for a successful installations is:
```
git version 1.8.4
```

###aludra.usc.edu
Aludra is one of the USC [Student Compute Facility](http://www.usc.edu/its/unix/servers/scf.html) clusters. git is already installed on aludra, however, you still need to configure your account to use it.

You can configure your account to use git by appending the following to your `~/.cshrc` file:

```bash
# git setup
if (-r /usr/usc/git/default/setup.csh) then
	source /usr/usc/git/default/setup.csh
endif
```

####Test Your installation
To see if git was properly configured you should run the following commands:

```bash
#Load the new configuration (you can logout, then login again instead)
source ~/.cshrc

git --version
```

The expected output is:
```
git version 1.6.4.2
```

####See You @ The Workshop!
