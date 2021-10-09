## CONTRIBUTING GUIDELINES

[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/SamarthMR/AI-ML-for-Newborn-Babies-in-Healthcare/issues)


<p align="center"><img src="https://i.ytimg.com/vi/qwvxfyddouQ/maxresdefault.jpg" width=600></p>

We want to make contributing to this project as easy and as transparent as possible, whether it's:<br>

- Reporting a bug :bug:

- Submitting a fix :mag_right:

- Proposing new features :bulb:

If you wish to contribute to this project, please raise an issue and wait for the project maintainers to approve it or give feedback before making a change.

This documentation contains a set of guidelines to help you during the contribution process. We are happy to welcome all the contributions from anyone willing to improve/add new scripts to this project. 



## Preliminaries

- Download and install the latest stable version of [Git](https://git-scm.com/downloads) 📥 for version control
- Create a [Github](https://github.com/) Account 📇


##   A. Setting up the Project

### 1.  Fork [this](https://github.com/CodeFlow201/Team-6) repository.

<p align="center"><img src="https://www.w3schools.com/GIT/img_github_fork.png" width="500" height="200" /></p>


### 2.  Clone your forked copy of the project.

To make a local copy of the forked repository, let’s first open up a terminal window.

We’ll use the `git clone`  command along with the URL that points to your fork of the repository.

You can alternatively copy the URL by clicking on the green “Code” button from your repository page. Once you click the button, you’ll be able to copy the URL by clicking the binder button next to the URL

You can copy the URL by clicking on the green “Code” button from your repository page. Once you click the button, you’ll be able to copy the URL by clicking the binder button next to the URL


<p align="center"><img width=35% src="https://www.w3schools.com/GIT/img_github_clone_url.png" width="500" height="200" /></p>
Once we have the URL, we’re ready to clone the repository. To do this, we’ll combine the git clone command with the repository URL from the command line in a terminal window:


````bash
$ git clone https://github.com/your-username/Team-6.git
````

### 3. Navigate to the project directory :file_folder: 


````bash
$ cd Team-6/
````








##  B. Contributing to the Project



### 1. Create a New Branch 

We'll create a new branch with the git branch command. Try to name it descriptively so that others working on the project understand what you are working on.
````bash
$ git branch new-branch
````


Now that our new branch is created, we will switch over to it using the git checkout command:
````bash
$ git checkout new-branch
Switched to branch 'new-branch'
````

At this point, you can now modify existing files or add new files to the project on your branch.


### 2. Perfom your desired changes to the code base.
Once you have modified existing files or added new files to the project, you can add them to your local repository, which you can do with the git add command. Let’s add the -A flag to add all changes that we have made:

````bash
$ git add -A
````
or
````bash
$ git add . 
````







- Comment any new code addition(s)

- Do not mess up the directory structure

- Preview your changes and test them properly before proceding ahead

<p align="center"><img width=35% src="https://media2.giphy.com/media/L1R1tvI9svkIWwpVYr/giphy.gif?cid=ecf05e47pzi2rpig0vc8pjusra8hiai1b91zgiywvbubu9vu&rid=giphy.gif"></p>




 


### 3. Commit your changes .
*The commit message is an important aspect of your code contribution; it helps the other contributors fully understand the change you have made, why you made it, and how significant it is. Additionally, commit messages to provide a historical record of the changes for the project at large, helping future contributors along the way.*


If you have a very short message, you can record that with the -m flag and the message in quotes:

Example:
````bash
$ git commit -m "Updated Readme.md"
[main (root-commit) e024518] Updated Readme.md
1 file changed, 1 insertion(+)...
````




### 4. Push the committed changes in your feature branch to your remote repo.


````bash
$ git push --set-upstream origin new-branch
````
### 5. Configure a Remote for the Fork

Next up, you’ll have to specify a new remote upstream repository for us to sync with the fork. This will be the original repository that you forked from. you’ll have to do this with the git remote add command.

````bash
git remote add upstream https://github.com/your-username/Team-9.git
````

In this example, `upstream` is the short name we have supplied for the remote repository since in terms of Git, “upstream” refers to the repository that you cloned from. If you want to add a remote pointer to the repository of a collaborator, you may want to provide that collaborator’s username or a shortened nickname for the short name.

### 6. Sync the Fork

Once you have configured a remote that references the upstream and original repository on GitHub, you are ready to sync your fork of the repository to keep it up-to-date.
To sync your fork, from the directory of your local repository in a terminal window, you’ll have to use the `git fetch` command to fetch the branches along with their respective commits from the upstream repository. Since you used the short name “upstream” to refer to the upstream repository, you’ll have to pass that to the command:

````bash
git fetch upstream
````

Switch to the local main branch of our repository:

````bash
git checkout main
Switched to branch 'main'
````

Now merge any changes that were made in the original repository’s main branch, that you will access through your local upstream/main branch, with your local main branch:

````bash
git merge upstream/main
````
### 8. Create Pull Request

At this point, you are ready to make a pull request to the original repository.

Navigate to your forked repository and press the `Create Pull Request`. Also add an appropriate title and description to your pull request that explains your changes and efforts done.


<img src="https://www.w3schools.com/GIT/img_github_fork_create_pull_request.png" width=600>
