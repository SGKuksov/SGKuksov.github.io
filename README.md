# SGKuksov.github.io

## Отправить последние изменения в удаленный репозиторий
``` bash
git add . # Add any untracked files
git commit -m "Update" # Commit the changes
git push # Push it to Github
```

## Создать ветку gh-pages
``` bash
git checkout --orphan gh-pages
git rm -rf .
touch README.md
git add README.md
git commit -m "Init gh-pages"
git push --set-upstream origin gh-pages
git checkout master
```

## Публикация на SGKuksov.github.io/your-reponame
``` bash
gulp deploy
```
