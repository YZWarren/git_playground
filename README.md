# playground
This is in Main branch, check

create branch
```
git remote add [branch_name] https://github.com/YZWarren/playground.git
git branch '[branch_name]'
git push [branch_name] [branch_name]
```

make changes in branch_name
```
git checkout [branch_name]
git add ./
git commit -m '[commit message]'
git push --set-upstream origin [branch_name]
```

merge target branch's history into current branch
```
git merge [target_branch_name]
```

delete target branch locally
```
git branch --delete [target_branch_name]
```

delete target branch remotely
```
$git push origin -d [target_branch_name]
```