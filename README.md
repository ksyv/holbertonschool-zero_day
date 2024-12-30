<div align="center"><img src="https://github.com/ksyv/holbertonschool-web_front_end/blob/main/baniere_holberton.png"></div>

# Git

## Table of Contents :

- [Resources](#Resources)
- [Learning Objectives](#Learning-Objectives)
- [Requirements](#Requirements)
- [Task](#Task)
    - [0. Create and setup your Git and GitHub account](#subparagraph1)
    - [1. Repo-session](#subparagraph2)
    - [2. Coding fury road](#subparagraph3)
    - [3. Collaboration is the base of a company](#subparagraph4)
    - [4. Collaboration: be up to date](#subparagraph5)
    - [5. HAAA what did you do???](#subparagraph6)
    - [6. Never push too much](#subparagraph7)
- [Authors](#Authors)

## Resources
### Read or watch:
* [Resources to learn Git](https://docs.github.com/en/get-started/getting-started-with-git/set-up-git)
* [About READMEs](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
* [How to write a Git commit message](https://cbea.ms/git-commit/)
* [Learning branching](https://learngitbranching.js.org/?locale=fr_FR)
* [Effective pull requests and other good practices for teams using GitHub](https://codeinthehole.com/tips/pull-requests-and-other-good-practices-for-teams-using-github/)

## Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:
* What is source code management
* What is Git
* What is GitHub
* What is the difference between Git and GitHub
* How to create a repository
* What is a README
* How to write good READMEs
* How to commit
* How to write helpful commit messages
* How to push code
* How to pull updates
* How to create a branch
* How to merge branches
* How to work as collaborators on a project
* Which files should and which files should not appear in your repo


## Requirements

* A README.md file at the root of the repo, containing a description of the repository
* A README.md file, at the root of the folder of this project (i.e. git), describing what this project is about
* Do not use GitHub’s web UI, but the command line to perform the exercise (except for operations that can not possibly be done any other way than through the web UI). You won’t be able to perform many of the task requirements on the web UI, and you should start getting used to the command line for simple tasks because many complex tasks can only be done via the command line.
* Your answer files should only contain the command, and nothing else

## More Info
### Install git
If git is not already installed on your terminal:

```
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install git
```
Note: If you’re already the ‘root’ user in the sandbox (e.g. your username starts with ‘root’), you can omit the ‘sudo’ from the commands above as you already have sufficient user permissions.

## Basic usage
At the end of this project you should be able to reproduce and understand these command lines:
```
$ git clone <repo>
$ touch test
$ git add test
$ git commit -m "Initial commit"
$ git push origin main
```

## Task
### 0. Create and setup your Git and GitHub account <a name="subparagraph1"></a>

#### Step 0 - Create an account on GitHub
You will need a GitHub account for all your projects. You can create an account for free [here](https://github.com/)

#### Step 1 - Create a Personal Access Token on Github
To have access to your repositories and authenticate yourself, you need to create a Personal Access Token on Github.

You can follow [this tutorial](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens) to create a token.

Once it’s created, you should have a token that looks like this:
<div align="center"><img src="https://github.com/ksyv/holbertonschool-zero_day/blob/main/img/git1.png"></div>

#### Step 2 - Update your profile on the Intranet
Update your Intranet profile by adding your Github username [here](https://intranet.hbtn.io/users/my_profile)

If it’s not done the Checker won’t be able to correct your work

#### Step 3 - Create your first repository
Using the graphic interface on the github website, create your first repository.

- Name: Look at the bottom of the project to see the name of the repository
- Description: This is my first repository as a full-stack engineer
- Public repo
- No README, .gitignore, or license
<div align="center"><img src="https://github.com/ksyv/holbertonschool-zero_day/blob/main/img/git2.png"></div>

#### Step 4 - Clone your repository
On the webterm of the sandbox, do the following:

- Clone your repository
```
root@896cf839cf9a:/# git clone https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/{YOUR_REPO}.git                  
Cloning into '{YOUR_REPO}'...
warning: You appear to have cloned an empty repository.
```
Replace {YOUR_PERSONAL_TOKEN} with your token from step 1

Replace {YOUR_USERNAME} with your username from step 0 and 1

Replace {YOUR_REPO} with the name of the repository at the bottom of the task

#### Step 5 - Create the README.md and push the modifications
- Navigate to this new directory.
```
root@896cf839cf9a:/# cd {YOUR_REPO}/
root@896cf839cf9a:/{YOUR_REPO}#
```
- Create the file README.md with the content My first readme.
```
root@896cf839cf9a:/{YOUR_REPO}# echo 'My first readme' > README.md
root@896cf839cf9a:/{YOUR_REPO}# cat README.md
My first readme
```  
- Add this new file to git, commit the change with this message “My first commit” and push to the remote server / origin
```
root@896cf839cf9a:/{YOUR_REPO}# git add .
root@896cf839cf9a:/{YOUR_REPO}# git commit -m 'My first commit'
[master (root-commit) 98eef93] My first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
root@896cf839cf9a:/{YOUR_REPO}# git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 212 bytes | 212.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/{YOUR_USERNAME}/{YOUR_REPO}.git
 * [new branch]      master -> master
```
Good job!

You pushed your first file in your first repository.

You can now check your repository on GitHub to see if everything is good.

### 1. Repo-session <a name="subparagraph2"></a>

Create a new directory called git in your repo.

Make sure you include a not empty README.md in your directory:

- at the root of your repository
- AND in the directory git
And important part: Make sure your commit and push your code to Github - otherwise the Checker will always fail.

### 2. Coding fury road <a name="subparagraph3"></a>

For the moment we have an empty project directory containing only a README.md. It’s time to code!

* Create these directories at the root of your project: bash, c, js
* Create these empty files:
    - c/c_is_fun.c
    - js/main.js
    - js/index.js
* Create a file bash/best with these two lines inside: #!/bin/bash and echo "Best"
* Create a file bash/school with these two lines inside: #!/bin/bash and echo "School"
* Add all these new files to git
* Commit your changes (message: “Starting to code today, so cool”) and push to the remote server

### 3. Collaboration is the base of a company <a name="subparagraph4"></a>

A branch is like a copy of your project. It’s used mainly for:

* adding a feature in development
* collaborating on the same project with other developers
* not breaking your entire repository
* not upsetting your co-workers

The purpose of a branch is to isolate your work from the main code base of your project and/or from your co-workers’ work.

For this project, create a branch update_script and in this branch:

* Create an empty file named bash/98
* Update bash/best by replacing echo "Best" with echo "Best School"
* Update bash/school by replacing echo "School" with echo "The school is open!"
* Add and commit these changes (message: “My personal work”)
* Push this new branch Tips
Perfect! You did an amazing update in your project and it’s isolated correctly from the main branch.

Oh wait, your manager needs a quick fix in your project and it needs to be deployed now:

* Change branch to main
* Update the file bash/best by replacing echo "Best" with echo "This School is so cool!"
* Delete the directory js
* Commit your changes (message: “Hot fix”) and push to the origin
Ouf, hot fix is done!

### 4. Collaboration: be up to date <a name="subparagraph5"></a>

Of course, you can also work on the same branch as your co-workers and it’s best if you keep up to date with their changes.

For this task – and only for this task – please update your file README.md in the main branch from GitHub.com. It’s the only time you are allowed to update and commit from GitHub interface.

After you have done that, in your terminal:

* Get all changes of the main branch locally (i.e. your README.md file will be updated)
* Create a new file up_to_date in the project directory (git) and in it write the git command line used
* Add up_to_date to git, commit (message: “How to be up to date in git”), and push to the origin

### 5. HAAA what did you do??? <a name="subparagraph6"></a>

Collaboration is cool, but not really when you update the same file at the same time…

To illustrate that, please merge the branch update_script to main: “Cool, all my changes will be now part of the main branch, ready to be deployed!”

HHHHHHHAAAAAAAA
```
CONFLICT (content): Merge conflict in bash/best
```
As you can see, you have conflicts between two branches on the same file.

Your goal now is to resolve conflicts by using the version of the branch update_script, and push the result to the origin.

At the end, you should have all your work from the branch update_script (new file and two updated files) and all latest main commits (new files, delete folder, etc.), without conflicts.

### 6. HAAA what did you do??? <a name="subparagraph7"></a>

Create a .gitignore file and define a rule to never push ~ files (generated by Emacs). [Tips](https://git-scm.com/docs/gitignore)
