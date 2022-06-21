### Migrate GIT [^1]

#### Before scripts
- Create new repo `URL_NEW_REPO`
- Ensure the main repo is named the same (main -> main, or master -> master)
#### Create a new clone (cleanest solution)
```bash
git clone --mirror URL_OLD_REPO
cd OLD_REPO
git push --mirror URL_NEW_REPO
```

#### On others
- Communicate this to all others
```bash
git remote set-url origin URL_NEW_REPO
```

[^1]: http://blog.plataformatec.com.br/2013/05/how-to-properly-mirror-a-git-repository/
