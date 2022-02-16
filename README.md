# WorkShop


## Install Git

### Windows:
[https://gitforwindows.org/](https://gitforwindows.org/)

### Mac

[https://sourceforge.net/projects/git-osx-installer/files/git-2.23.0-intel-universal-mavericks.dmg/download?use\_mirror=autoselect](https://sourceforge.net/projects/git-osx-installer/files/git-2.23.0-intel-universal-mavericks.dmg/download?use_mirror=autoselect)

### Linux
   - **Debian/Ubuntu:** sudo apt-get install git-all
   - **Fedora:** sudo dnf install git-all

## Git Config

Now that you have git installed, you need to do some configuration: 

 - _git config --global user.name &quot;John Doe&quot;_
 - _git config --global user.email johndoe@example.com_
 
 Make sure to replace the user name and email by yours.
 
## Your first project
Create a folder 'engbio' and inside that same folder run the command:

- _git init

This will create a '.git' folder with all that git needs to perform version control.

Create a new file _README.md_ with any editor of your choice. You might also create the file from the command line using
`echo "Some Text" >> README.md `. You may now stage the new file and commit the changes.

- _git add README.md_
- _git status_
- _git commit -m &quot;first commit&quot;_

You may want to verify the project status using:

- _git status_

Now let us create a branch for the project.Branches allow developers to diverge from the production version to fix a bug or add a feature without modifying the existing version.
A project should always have a 'main' or 'master' branch, so we need to create it.

- _git branch_
- _git branch -M main_
- _git branch_

## Using Github

Create a GitHub account and a new project, &#39;engbio&#39;.

Go to Settings/Developer settings and create a new access token. Add a note identifying the purpose, generate, copy the token and save it into a file.

Now let us configure git to define a remote origin

- _git remote add origin_ [_https://github.com/vmsapereira/engbio.git_](https://github.com/vmsapereira/engbio.git)

And push the commits

- _git push -u origin main_

## Git clone

Another way to create a git project is to clone an existing one

- _git clone https://github.com/vmspereira/Dummy.git_

When cloning a repository, without specifying a branch, all the branches are cloned.

You can list the branches and switch branches with the git commands:

- _git branch -a_
- _git checkout workflow_

Now let us merge the workflow branch into the master

- _git checkout master_
- _git merge workflow_

Create a new &#39;Dummy&#39; repository on your GitHub

- _git remote add myorigin https://github.com/vmsapereira/Dummy.git_
- _git branch -M master_
- _git push -u myorigin master_
