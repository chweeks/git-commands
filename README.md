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
