# Nuances of git

'Nuances of git' repository created to learn Git and GitFlow.

## Commands list

1. Shows info about *command*

`git command -help`

2. Initializes Git repository

`git init`

3. Shows repository status

`git status`

useful flags:

*--short* - shows short status description

4. Adds files changes to repository (new, modified and deleted)

`git add file_name`

useful flags:

*--add* or *-A* - adds changes of all files

5. Commits changes

`git commit -m "commit message"`

This command must be **ALWAYS** used with *-m* flag and short, descriptive message about added changes (Answer these questions when commiting: what was added? What was fixed? What was updated? What was changed?).

6. Shows history of commits for repository

`git log`

7. Creates new branch with *branch-name* in repository

`git branch branch-name`

8. Shows all local branches

`git branch`

Current branch tagged with (*)

useful flags:

*-a* - shows all local and remote branches
*-r* - shows all remote branches

9. Deletes branch with *branch-name*

`git branch -d branch-name`

10. Renames branch

`git branch --move bad-branch-name correct-branch-name`

11. Switches branch to *branch-name*

`git checkout branch-name`

useful flags:

*-b* - allows to create a branch and switch to this one instantly

Example:

`git checkout -b dev`

will create and switch to branch *dev*

12. Merges current branch with *branch-name*

`git merge branch-name`

13. Adds remote repository to local repository

`git remote add origin URL`

Where *URL* - URL of remote repository of github, gitlab or something else.

14. Pushes *branch-name* to the origin url and set it as the default remote branch

`git push -u origin branch-name`

15. Pulls changes from remote repository

`git pull origin branch-name`


16. Deletes remote branch with *branch-name*

`git push origin --delete branch-name`

## GitFlow

The GitHub flow works like this:

- Create a new Branch
- Make changes and add Commits
- Open a Pull Request
- Review
- Deploy
- Merge
