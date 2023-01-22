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
    
    if `gh` not install, run `conda install gh --channel conda-forge`

## create a new repository on the command line
```
echo "# git_playground_test" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/YZWarren/git_playground_test.git
git push -u origin main
```

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
git push origin -d [target_branch_name]
```