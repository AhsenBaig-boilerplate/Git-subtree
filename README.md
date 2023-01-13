# Git-subtree
Git Demo subtree
## subtree merge
``` 
git remote add -f spoon-knife https://github.com/AhsenBaig-boilerplate/Git-subtree-Spoon-Knife.git
```

```
git merge -s ours --no-commit --allow-unrelated-histories spoon-knife/main
```

```
git read-tree --prefix=spoon-knife/ -u spoon-knife/main
```

```
git commit -m "Subtree merged in spoon-knife"
```

### Synchronizing with updates and changes
When a subproject is added, it is not automatically kept in sync with the upstream changes. You will need to update the subproject with the following command:

```
git pull -s subtree spoon-knife main
```

## Resources
- [About Git subtree merges](https://docs.github.com/en/get-started/using-git/about-git-subtree-merges)
- [Original Spoon-Knife](https://github.com/octocat/Spoon-Knife.git)
