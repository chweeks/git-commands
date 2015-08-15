                                       git-commands

            Commands                        |                       Description
______________________________________________________________________________________

Create:                                     |
  
$ git clone ssh://user@github.com/repo.git  | Clone existing repository
$ git init                                  | Create new local repository
                                            |
Local Changes:

$ git status                                | List changed files in your working directory
$ git diff                                  | Changes to tracked files
$ git add .                                 | Add all existing changes to next commit
$ git add -p <file>                         | Add changes in <file> to next commit
$ git commit --all                          | Commit all local changes in tracked files
$ git commit                                | Commit staged changes
$ git commit -m 'text'                      | Commit staged changes with comment 'text'
$ git commit --amend                        | Change last commit
                                            |
Commit History:

$ git log                                   | Shows all commits (newest-oldest)
$ git log-p <file>                          | Shows changes to <file>
$ git blame <file>                          | Who, what and when <file> changed
                                            |
Branches:

$ git branch -av                            | List all branches
$ git checkout <branch>                     | Change to <branch> 
$ git branch <new-branch>                   | Create new <branch> 
$ git checkout --track <remote/branch>      | Create tracking <branch> from <remote> branch
$ git branch -d <branch>                    | Delete local <branch>
                                            | 
Update & Publish:

$ git remote -v                             | List all current remotes
$ git remote show <remote>                  | Show <remote> info
$ git remote add <name> <url>               | Add new remote repo with <name> to <url>
$ git fetch <remote>                        | Download all changes from <remote> but don't add to HEAD
$ git pull <remote> <branch>                | Download all changes from <remote> and merge with HEAD
$ git push <remote> <branch>                | Publish local changes to repo
$ git branch -dr <remote/branch>            | Delete <branch> on <remote>
                                            |
Merge:

$ git merge <branch>                        | Merge <branch> into HEAD
$ git rebase <branch>                       | Rebase HEAD onto <branch>
$ git rebase --abort                        | Abort a rebase                             
$ git add <resolved-file>                   | Add manually resolved files
$ git rm <resolved-file>                    | Remove manually resolved files
                                            |

Undo:

$ git reset --hard HEAD                     | Discard all local changes in working directory
$ git checkout HEAD <file>                  | Discard local changes in <file>
$ git revert <commit>                       | Revert a <commit> (replace with new one)
$ git reset --hard <commit>                 | Reset HEAD to previous <commit> and discard new changes since <commit>
$ git reset <commit>                        | Reset HEAD to previous <commit> keep new changes as unstaged
$ git reset --keep <commit>                 | Reset Head to preivous <commit> keep new changes asstaged
                                            |