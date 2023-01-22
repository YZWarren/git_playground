# playground
This is in Main branch, check

## Adding a local repository to GitHub with GitHub CLI
1. In the command line, navigate to the root directory of your project.
2. Initialize the local directory as a Git repository.
```
git init -b main
```
3. Stage and commit all the files in your project.
```
git add . && git commit -m "initial commit"
```
4. Create remote repo from CLI `gh repo create` and follow prompts

if not logged in in current machine, first run `gh auth login` and follow prompts

## create branch
```
git remote add [branch_name] https://github.com/YZWarren/playground.git
git branch '[branch_name]'
git push [branch_name] [branch_name]
```

## make changes in branch_name
```
git checkout [branch_name]
git add ./
git commit -m '[commit message]'
git push --set-upstream origin [branch_name]
```

## merge target branch's history into current branch
```
git merge [target_branch_name]
```

## delete target branch locally
```
git branch --delete [target_branch_name]
```

## delete target branch remotely
```
$git push origin -d [target_branch_name]
```