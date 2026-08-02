### Branch Create

```bash
git branch dark-mode
```

Branch list:

```bash
git branch
```

Output:

```bash
* main
  dark-mode
```


### Branch Change

```bash
git switch dark-mode
```

Old way:

```bash
git checkout dark-mode
```

### Shortcut: Create + Switch

```bash
git switch -c dark-mode
```

### Real Example

Current:

```bash
main
```

Create feature branch:

```bash
git switch -c login-page
```

Code.....

Commit:

```bash
git add .
git commit -m "Added login page"
```

Graph:

```
main
  \
   login-page
```

### Merge

Feature complete hole:

```bash
git switch main
git merge login-page
```

Graph:

```
main
 |
 └── login-page changes
```

### Push Branch to GitHub

```bash
git push -u origin login-page
```

### Commands Summary

```bash
git branch                 # list branches
git switch branch-name     # switch branch
git switch -c new-branch   # create + switch
git merge branch-name      # merge branch
git branch -d branch-name  # delete branch
git push -u origin branch  # upload branch
```

* Feature shesh hole `main` e merge
* Production project-e sorasori `main` e code na likha bhalo practice. 
