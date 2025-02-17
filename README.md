# WorkTree
WorkTree

### Guide to setup Github with WorkTree

With a Repository that already exist
```bash
git clone https://github.com/MrAmericanMike/WorkTree.git WorkTree/master
cd WorkTree/master
git worktree add ../cool cool
```

If branch `cool` doesn't exist yet use:
```bash
git worktree add ../cool
```

### Documentation

https://git-scm.com/docs/git-worktree


## Add independent branches as Worktrees

```bash
git checkout --orphan 1.21.4-fabric

git reset .

git clean -fxfd

git commit --allow-empty -m "1.21.4-fabric"

git checkout master

git worktree add ../1.21.4-fabric 1.21.4-fabric
```
