## Terminology
<hr />

* **Merging**:  The act of combining two different branches together.

## Overview
<hr />

* To merge one branch into another, you must first navigate to the branch you'd like to introduce new code into.

* Once located in that branch, the command `$ git merge <branch-name>` will merge the commits from the outside branch into the current branch.

* If the two branches don't contain edits to the same areas, Git will be able to merge these two branches automatically.

* If two branches contain edits to the same areas of code, this will result in a merge conflict, and Git will request you resolve it manually. We'll explore merge conflicts in detail later on. 
