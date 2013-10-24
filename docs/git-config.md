#Git Configuration

After [installing git](git-setup.md) on your system, the next step is to customize your own git environment. This is a one-time step that you don't need to repeat unless you want to change the existing configuration.

You will define your git _profile_ in your development environment. This is **important** because your profile information is used to annotate your _contributions_ to a repository/project. Although this may not seem like a big deal when you are the only one committing to a repository, it is of the utmost importance once you work on a group project because this information is the basis used to calculate [your contribution](https://github.com/jquery/jquery/contributors) to a project.

The most basic information to setup is:
  + Name, e.g. `Tommy Trojan`
  + Email, e.g. `ttrojan@usc.edu`
  + Editor for commit messages, e.g. `vi`, `emacs`, `notepad`
  + Git message colors (make it pretty-er)
  + Properly handle [new lines](http://en.wikipedia.org/wiki/Newline#Common_problems)

Configuration is performed manually through the command line. To start the configuration you would need to launch:

  + MacOS or Linux: Terminal
  + Windows: Git Bash

```bash
#Set your name and email
git config --global user.name "Tommy Trojan"
git config --global user.email "ttrojan@usc.edu"
```

#####Git CLI Interface
By default, git does not color its output. Pretty printing git messages makes it easy read the output and take proper actions. You can enable colors for interactive use of git by:

```bash
#Lets get pretty colored output!
git config --global color.ui auto
```

#####Git Message Text Editor
When committing code in git, the system requires a commit message. If a message is not provided via the commandline, git will launch the Operating System's default text editor prompting you for a message. You can customize this action using the following configuration directive:

```bash
#Pick your editor of choice to edit commit messages (not code)
# Note that you should pick an editor that is installed on your machine
git config --global core.editor emacs
```

Here, git will automatically launch `emacs`. You may want to change that to your editor of choice. Here are some examples (you only need one):

```bash
#vim (if installed on your OS)
git config --global core.editor vim

#TextMate in MacOS
#  configuration notes:
#  http://blog.macromates.com/2005/textmate-shell-utility-tmmate/
git config --global core.editor "mate -w"

#Notepad in Windows
git config --global core.editor "c:/Windows/notepad.exe"

#Notepad++ in Windows
# Make sure the path to Notepad++ is correct on your machine
git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst -notabbar -nosession -noPlugin"
```

#####Let Git Handle New Lines
Operating Systems implement [new lines](http://en.wikipedia.org/wiki/Newline#Common_problems) differently. Here you will configure git to automatically normalize the line feed (`LF`) to properly match the platform. Please use the proper configuration command for your OS:

  + Linux & MacOS:
  
```bash
#LF Normalization (Linux & MacOS)
git config --global core.autocrlf input
``` 

  + Windows:
  
```bash
#LF Normalization (Windows)
git config --global core.autocrlf true
```

#####Check Your Work
```bash
#List local git configuration options
git config --list
```
