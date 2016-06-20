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
The Git-Plus package uses git's config file to get your GitHub info so it can add, commit and push your files to GitHub.  So once Git is working open your Terminal and type:
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

#### 5. Install Git-Plus package
You're almost there!  The last step is to install the Git-Plus package so that you can do everything git from Atom itself.  HOW COOL IS THAT? :sunglasses:  So open Atom and in the top menu bar go to `Atom > Preferences`.  A new tab should open with a Settings page.  Here you can click the Install button and in the text field type `git-plus`.  Press the `Package` button on the right and the first result should be by the author `akonwi`, on this package click the blue install button and the package should install.  Once finished you can close that tab, open a new blank tab and press <kbd>command</kbd>+<kbd>shift</kbd>+<kbd>H</kbd>.  If this doesn't pull up a command window at the top then the package didn't install properly and you should uninstall and reinstall.
