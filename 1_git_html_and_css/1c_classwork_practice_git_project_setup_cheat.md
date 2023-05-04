## Terminology
<hr />

* **Initialize**: In Git, we can initialize a new, empty repository to track changes to the project directory by running `git init`. We should always run this command in the top level of the project directory.

* **Global**: A configuration option that refers to every directory in every location of the device.

* **Hidden files**: These are files on your machine that are not listed with an `ls` terminal command. Instead, you can see them with the `ls -a` terminal command. The `.git` directory is hidden by default.

## Daily Git Workflow
<hr />

This workflow is only for students pair programming in person at Epicodus.

### Set up name and email

#### On Personal Computers

Git needs your name and email to be able to connect local work on our machines to a remote GitHub account. To set up your Git credentials on your personal computer, you can do this just once by setting up **global** credentials that will be applied to all projects. 

```shell
$ git config --global user.name "Padma Patil"
$ git config --global user.email padma@email.com
```

#### On Shared Computers On Campus at Epicodus

On shared computers on campus at Epicodus, at the beginning of each class session **one** student in a pair will set up **global** Git credentials. The instructions on how to do this are the same as above. Note that these global Git credentials will be wiped when students shut down the computers at the end of every work day. 

Later on, the same student who set up the global Git credentials will use other Git commands to save the local project on their remote GitHub account. Then, the other student(s) in the pair will copy that project, saving it to their own remote GitHub account. We'll go over this workflow in detail when we are ready for this step.

#### Sharing Authorship on Shared Projects

Later on we will learn how to use a **commit trailer** when creating **commits** to share authorship among multiple people. 

### Create a new project directory with Git repository

In terminal:

```shell
$ cd Desktop
$ mkdir hello-world
$ cd hello-world
$ git init
```

## Git Commands
<hr />

* `git init`:   Initializes new local Git repository.

* `git config --global user.name ___`:  Globally configures Git profile for entire device (use only on your personal machine).
