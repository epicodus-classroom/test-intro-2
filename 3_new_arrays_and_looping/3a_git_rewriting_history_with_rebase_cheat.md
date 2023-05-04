## Terminology
<hr />

* **Rebase**:  The act of moving a branch to a new base commit (essentially just moving a branch from one commit to another).

* **Squashing**:  The act of combining multiple commits together into one.

## Commands
<hr />

* `$ git log --oneline`:  Returns a repository's log of commits, each condensed to a single line.

* `$ git commit --amend -m "updated commit message here.`:  Modifies a repository's most recent commit message with the new message provided.

* `$ git rebase -i`:  Changes commit messages and combines multiple commits by "squashing" them together:
  * rewrite commit messages by changing `pick` to `reword`
  * squash one or more commit messages by changing `pick` to `squash`

## Examples
<hr />

See a project's commit history with the `git log` command. Add the `--oneline` flag to display the history in an easier to read format:

```shell
$ git log --oneline
d7e33de something css related
32ccc0b do something with html
9db82b6 update readme
79e9de2 add readme
827ad58 add initial files
```

Amend the most recent Git commit:

```shell
$ git commit --amend -m "add styling to main page"
```
