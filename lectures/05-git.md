Git Example
===========

Getting Started
---------------

- `git init` is used to to create a repository
- Create a regular repositories in directory `a`
- Create a bare repo (`git init --bare`) in `origin`

Examining State
---------------

- `git status` will show the current state of the repository

Initial Commit
--------------

- Add a file with some code to the repo in `a`
    1. Create a new file and give it some content
    2. Use `git add {filename}` to add the content from the working tree to the index
    3. Use `git commit {filename} -m "{message"}` to create a new commit recording these changes

Adding a Remote
---------------

- Add the origin repository as a remote
- `git remote add origin ../origin`
- Use `git remote` to list remotes

Pushing
-------

- Pushing allows us to update remotes refs from our local refs
- `git push` performs this task
- We first need to set the upstream branch using `git push --set-origin origin main`

Cloning
-------

- Repositories can be copied using clone
- Use a command such as `git clone {original} {new}` to clone a repository
- Create a cloned repository `b` using `git clone origin b`

Update B
--------

- Add a new change from `b`
- Push it to origin
- Switch back to `a` and pull your change

Merge Conflicts
---------------

- Create a change in `a` and push it
- Create a change in `b` without pulling first and push it
- Use `git pull` to initiate merging the changes

Resolving Conflicts
-------------------

- Simple merges will be resolved automatically
- Conflicting files can be shown using `git status`
- Conflicting files will show both changes and can be manually edited to resolve the conflict
- Use `git add` to mark as fixed and `git commit` to create a merge commit

Exploring History
-----------------

- `git log` shows history
- `--oneline` removes some info
- `--graph` shows a basic graphical representation on the left
