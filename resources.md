# Resources

## Infrequently Used Git Commands (Once Per Project Repo)
* `git init` - initialize a Git repository within a directory (aka 'folder')
* `git clone <url>` - clone a repository at url (don't type brackets)

## Frequently-used Git Commands

### Check status of repository, changes
* `git status` - Show changed files, contents of index
* `git diff HEAD <file>` - Show difference between file in working tree and file in repo

### Stage files for commiting
* `git add .` - add all files to the index for commiting
* `git add <list of files>` - add a particular file or files to the index (don't type brackets)

### Commit staged files
* `git commit -m "Commit message"` - Commit staged files in the index; attach message in quotation marks

### Stage and commit simultaneously (be careful)
* `git commit -am "Commit message" - 

* `git log` - Show verbose log of history
* `git log --pretty=oneline` - Show one-line log of history
* `git log --pretty=oneline --abbrev-commit` - Show one-line log with shorter SHA-1 hash

### Revert to last commited version of file
* `git checkout <file name>` (don't type brackets)

### Branches and Branching
* `git branch` - Show all local branches; `*` marks current branch
* `git branch <branch name>` - Create a new branch (don't type brackets)
* `git checkout <branch name> - Switch to a different branch (don't type brackets)

### Merging
1. Checkout the branch you wish to merge onto (e.g., `git checkout master`)
2. Perform the merge (e.g., `git merge working`)
3. If there are conflicts, find them in the files and fix; run `git add <list of conflicting files>`
4. Finish the merge by running `git commit` (No message; one will be created automatically)

* If you want to back out of the merge if there are conflicts, run `git reset --hard`

### Cherry-Picking
This pulls only the commits you want from another branch, using the first 5 or 6 characters of the commit's SHA-1 hash.
1. Checkout the branch you with to cherry-pick to (e.g., `git checkout master`)
2. Perform the cherry-pick: `git cherry-pick <hash>` (e.g., `git cherry-pick 9fb012`)
3. If there are conflicts with the cherry-pick, find them in the files and fix; run `git add <list of conflicting files>`
4. Finish the cherry-pick by running `git commit`

* If you want to back out of the cherry-pick if there are conflicts, run `git reset --hard`

### Tagging
* `git tag <tag name>` - Creates a tag of `tag name` (no brackets) based on current position in the repository

### Working remotely
* `git remote add <remote name> <url>` - Added a remote of `remote name` at `url` (no brackets); e.g., `git remote add origin git@github.com:account/repo.git`
* `git push <remote name> <branch or tag>` - Push a particular tag or branch to the remote from your current place in the repository, e.g., `git push origin master`
* `git pull <remote name> <branch>` - Pull a particular branch from the remote, e.g., `git pull origin master`

# Resources and Further Reading

## Websites and Books
* Git Manual Page. http://www.kernel.org/pub/software/scm/git/docs/
* Chacon, Scott. Pro Git. Apress, 2009. Web version: http://progit.org/book/ Git Repo: https://github.com/progit/progit || git clone git://github.com/progit/progit.git
* Swicegood, Travis. _Pragmatic Version Control Using Git_. Pragmatic Bookshelf, 2008.
* Swicegood, Travis. _Pragmatic Guide to  Git_. Pragmatic Bookshelf, 2010. [More of a quick reference guide.]

## Tutorials
* http://help.github.com/s
* Stolley, Karl. Git Tutorial. http://wiki.karlstolley.com/GitTutorial
* Stolley, Karl. Git Fu. http://courses.karlstolley.com/530/GitFu

