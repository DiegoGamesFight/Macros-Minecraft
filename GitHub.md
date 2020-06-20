branch = ramo;

commit = enviar informação/arquivo;

pull request = solicitação de recebimento;

fetch = buscar;

merge = fundir (branch's);

- `git clone <http link folder>`
- `git clone https://github.com/DiegoGamesFight/Macros-Minecraft.git`
- `git status` (Show the changed files in the branch)
- `git add <file_name> <file_name2>...` (Add the file specified in the commit)
- `git commit -m "message"` (Commit the files with the parameter '-m' to put a message)
- `git push origin <branch_name>` (Fetch the commit in the branch)

## Branch
branch = "Copy of the master branch to do test/modify/change, etc."
- `git branch` (Show all the branch's in the repository)
- `git branch <branch_name> -D` (Delete the branch) 
- `git branch <branch_name>` (Create a new branch in the repository)
- `git checkout <branch_name>` (Switch to the specified branch in the repository)

## Useful commands:
- `git branch --v` (This will list out your local branches with more information including what each branch is tracking and if your local branch is ahead, behind or both.)

```vim
   iss53     7e424c3 [origin/iss53: ahead 2] Add forgotten brackets
   master    1ae2a45 [origin/master] Deploy index fix
 * serverfix f8674d9 [teamone/server-fix-good: ahead 3, behind 1] This should do it
   testing   5ea463a Try something new
```

## Pull request
Step 1: From your project repository, bring in the changes and test.
- `git fetch origin`
- `git checkout -b test origin/test`
- `git merge master`

Step 2: Merge the changes and update on GitHub.
- `git checkout master`
- `git merge --no-ff test`
- `git push origin master`

