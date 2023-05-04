## Pair Commit Workflow
<hr />

### Add file(s) to track in Git

In terminal:

```shell
$ git add hello-world.html
```

or if multiple files should be added the `.` can be used to add all files:

```shell
$ git add .
```

### Commit

In terminal:

```shell
$ git commit -m "add a short, descriptive present tense commit message here describing the changes made"
```

### Updating the Master Branch to the Main Branch

Your global configuration should be set up so that all projects default to a `main` branch, not a `master` branch. See the [Git Configurations](https://www.learnhowtoprogram.com/introduction-to-programming/getting-started-with-intro-to-programming/git-configurations) lesson if you need to update your global Git configuration.

You can also update the default branch in an individual project as well. After making your first commit, run the following command:

```
$ git branch -M main
```

## Git Commands
<hr />
In this reference, examples in brackets `[xxx]`, should be entirely replaced by what is indicated (do not leave brackets).  

### Set up configurations

* `git config user.name "[name]"`:  Sets a SINGLE user name for all commits in one project. The command must be run in the root directory of that project. You should always use a local configuration on Epicodus machines.

* `git config user.email "[email address]"`: Sets a SINGLE user name for all commits in one project. The command must be run in the root directory of that project. You should always use a local configuration on Epicodus machines.

* `git config --global user.name "[name]"`: Sets a SINGLE user name for all commits on a global level. Only do this on your personal machine. You will only need to run this command once.

* `git config --global user.email "[email address]"`: Sets a SINGLE email for all commits on a global level. Only do this on your personal machine. You will only need to run this command once.


### Committing

* `git add .`:  Adds ALL files with changes to be committed.

* `git add [file]`:  Adds the named file to be committed.

* `git commit -m "[message]"`:  Records all of the staged files permanently to the version history; message should describe the changes finishing the phrase "This commit will...".

*  Example:  `git commit -m "add AJAX functionality to the comments form"`

### Reviewing Git Information

* `git log`:  Lists commit history for the current branch.

* `git status`:  Lists the files where changes have been made to be committed.
