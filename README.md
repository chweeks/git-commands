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

