## Terminology
<hr />

* **Vim**:  Default text editor designed for use from the command line.

* **Global**:  An option in many command line commands that applies the changes everywhere instead of just in the current directory.

## Configurations
<hr />

### Make Visual Studio Code Your Default Git Editor

```
$ git config --global core.editor "code --wait"
```

### Color Output

```shell
$ git config --global color.ui true
```

### Git Ignore Files

* Add this file to your home directory:

<div class="filename">.gitignore_global</div>

```shell
# OS generated files #
######################
.DS_Store
.DS_Store?
._*
.Spotlight-V100
.Trashes
ehthumbs.db
Thumbs.db
```

* Run this command to use it:

```shell
$ git config --global core.excludesfile ~/.gitignore_global
```
