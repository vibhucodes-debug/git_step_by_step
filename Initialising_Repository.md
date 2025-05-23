# Basic steps in initialising a Repository


### Setting Up

> git config --global user.name "Vaibhav Sharma"

> git config --global user.email "vaibahvsharma2124@gmail.com"

> git config --global core.editor "code --wait"
  - Set the default code editor as VS Code.


### Initialising

  > `git init`
    - Initialise an empty repo in the current folder

*Git creates a hidden folder called .git inside your project. This is where Git stores all the information it needs to track your files and history.*  

  > `git status`
    - The `git status` command displays the state of the working directory and the staging area.

### Staging 

  *The staging environment (or staging area) is like a waiting room for your changes. We use it to tell git exactly which files to include in the next commit*

  > `git add <filename>`
    - Add a file in the staging area.
      
  > `git add --all` OR `git add -A`
    - Add all files to staging area.
  >  `git restore --staged <filename>`
    - Remove a file from the staging area.

### Commit 

  * A  `commit` is like a save point in our project. It records a snapshot of our files at a certain time, with a message describing what changed. We can always go back to a previous commit if we need.*


  > `git commit -m "messaging"`
    - Commit staged changes with a message.

  > `git commit -m -a "messaging"`
    - Commit all tracked files and, skipping staging.

  > `git log`
    - Display the commit history
    *Note: This commits all the modified, and deleted items, but not **the new tracked files**.


### Branching 

> `git branch new-branch`
  - To create a new branch.

> `git checkout new-branch`
  - To shift move on another branch.

*Any commits you make on this branch will be separate from the main branch and won’t affect it. This allows you to work on new features or bug fixes without disrupting the stability of the main branch.*

**Steps invovled in merging 'new-branch' to the 'main' branch:**

- `git checout main`
- `git merge new-branch`

  
  
  

