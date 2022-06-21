### Migrate GIT

#### Before scripts
- Create new repo `URL_NEW_REPO`
- Ensure the main repo is named the same (main -> main, or master -> master)
#### On latest pulled origin
```bash
# Check remotes
git remote -v

# Mirror current repo to new remote
git push --mirror URL_NEW_REPO
git remote set-url origin URL_NEW_REPO
```

#### On others
- Communicate this to all others
```bash
git remote set-url origin URL_NEW_REPO
```
