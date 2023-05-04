## Terminology
<hr />

* **Local**:  In Git terms, local means located on the device that you are using.

* **Remote**:  In Git terms, this means located outside of the device you are using; for example, GitHub.

* **README**:  A file that provides more details information about a GitHub repository's code.

* **Push**:  Copy the code from a local Git repository to a remote repository.

* **Main**: The main copy of a Git repository on a local machine, also known as the main branch. Traditionally, this was called the "master" branch but this terminology has been updated due to its negative connotations.

* **Clone**:  To make a copy of a repository from Github on a local machine.

* **Origin**:  The default nickname given to the GitHub remote repository when it is cloned.

## Git Remote Commands
<hr />

* `$ git remote add [remote name] [remote URL]`:  Sets up a new remote location with a name and location.  

Example: This command adds a new remote called "al" located at "https://github.com/epicodus-lessons/hello-world":

```shell
$ git remote add al https://github.com/epicodus-lessons/hello-world
```

* `$ git remote -v`: Shows the names and URLs for all of the remote repositories that the project's Git repository has stored.

* `$ git push [remote name] [branch name]`: Copies the code to the remote repository from the local Git repository.

* `$ git clone [remote URL]`:  Copies the code and commit history from a remote repository to a local repository.

## Tips
<hr />

* Be sure that you are not cloning a project inside of an existing local repository. In other words, you should _not_ be inside of a project directory when you run the `git clone` command. Otherwise you'll end up with one git repository inside of another.
