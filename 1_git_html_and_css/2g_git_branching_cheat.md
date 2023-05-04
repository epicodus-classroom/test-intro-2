## Terminology
<hr />

* **Branching**:  The act of making multiple copies of the same code in the same project. Usually in order to do different things with the same code base, or to allow multiple people to work on the same code at the same time.

* **Branch**:  Another copy of your code

* **Main Branch**:  Like the "final draft" of your code.

* **Feature Branches**: A common term for branches that are _not_ `main`. Usually branches meant for experimenting with new features before adding them to the final version of the project.

## Tips
<hr />

* The `$ git branch` command with nothing after it will display all branches in a project. The branch you're currently located in will be denoted with an asterisk `*`.

* The `$ git branch` command with a branch name after it (ie: `$ git branch <name-of-new-branch>`) will create a new branch of the name you specify. Branch names should be short and meaningful, and describe the reason for the branch.

* We can switch which branch we're viewing by using the `$ git checkout` command with the name of the branch we'd like to see. For instance, `$ git checkout blue_theme` will move us to a branch named `blue_theme`. 
