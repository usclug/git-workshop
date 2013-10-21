#Git Installation Instructions

##Linux
Almost all major Linux distributions have git as a package that you can install using their standard package manager software.

  + Debian-based distro such as Ubuntu and Mint Linux use:
```bash
sudo apt-get install git
```

  + Fedora & CentOS can use:
```bash
sudo yum install git-core
```

###Test Your installation
To see if git was properly installed you should run the following command in a terminal window
```
git --version
```

The expected output for a successful installations is
```
git version 1.8.4
```

##MacOS
There are multiple ways to install git on MacOS. The easiest way is to install the Apple pre-packaged version of git that comes with [Xcode](https://developer.apple.com/xcode/). The installation process is as follows:

  1. Install [Xcode](https://itunes.apple.com/us/app/xcode/id497799835) from the [Mac App Store](https://itunes.apple.com/us/app/xcode/id497799835)
  1. Install the **Command Line Tools** for Xcode using one of the following two methods:
    + Xcode &rarr; Preferences &rarr; Downloads &rarr; Components &rarr; Click `install` next to the Command Line Tootls; or
    + Download and install the Command Line Tools package from the [Apple Developers Downloads](https://developer.apple.com/downloads) page.
