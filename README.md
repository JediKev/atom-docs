# ⚛ Atom Docs

### Description
Documentation for setting up Git, create/connect a GitHub account, installing Atom editor and installing Git-Plus package for Git commands without terminal.

#### 1. Install Atom
Head over to the [Atom](https://atom.io/) website and click the download button on the front page. Once downloaded open the `.zip` file and it should un-pack itself.  Once un-packed, you can open Atom and use it.

#### 2. Create/Connect GitHub account
Head over to the [GitHub join page](https://github.com/join) and make a Free account.  If you choose to you could go through the steps of checking, generating, and adding an [SSH key](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/) to GitHub so that Atom will not prompt for credentials every time you push to GitHub.  This is not necessary by any means but it does make workflow a lot faster.

#### 3. Set up Git
Git usually comes pre-installed on most Mac machines.  The way you can check is by typing in your Terminal:
```
$ git --version
```
It should return a result like:
```
$ git --version
  git version 2.5.4 (Apple Git-61)
```
If you get a result then head to the next step.  If you get an error or nothing happens then it isn't installed and you can head to the [Git Getting-Started Guide](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and follow the instructions to download/install Git.

#### 4. Set up .gitconfig
Atom uses git's config file to get your GitHub info so it can add, commit and push your files to GitHub.  So once Git is working open your Terminal and type:
```
$ atom ~/.gitconfig
```
This should open a file in Atom called `.gitconfig`.  Within this file add the following to the bottom:
```
[user]
        name = UserName
        email = example@example.com
```
Replacing `UserName` with your GitHub Username and `example@example.com` with your GitHub email address. If this stuff already exists just make sure it matches your GitHub info.
