# WorkShop


## Install Git on Windows:

[https://gitforwindows.org/](https://gitforwindows.org/)

## Install Git on Mac

[https://sourceforge.net/projects/git-osx-installer/files/git-2.23.0-intel-universal-mavericks.dmg/download?use\_mirror=autoselect](https://sourceforge.net/projects/git-osx-installer/files/git-2.23.0-intel-universal-mavericks.dmg/download?use_mirror=autoselect)

Install Git on Linux
   - **Debian/Ubuntu:** sudo apt-get install git-all
   - **Fedora:** sudo dnf install git-all

## Git Config

 - _git config --global user.name &quot;John Doe&quot;_
 - _git config --global user.email johndoe@example.com_
 - _git config –list_
 - _git config –show-origin_

## Git init

Create a new folder &#39;engbio&#39; and inside this folder:

- _git init_

Create a README.md file

- _git add README.md_
- _git commit -m &quot;first commit&quot;_
- _git status_
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
