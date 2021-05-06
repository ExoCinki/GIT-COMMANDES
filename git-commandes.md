## Lister les branchs

```shell
# Permette de voir toutes les branches existantes (local et remote)
git branch -a
```

## Créer une branch

```shell
# Deux lignes: créer et basculer sur la nouvelle branch
git branch nom_de_ma_branch_nouvelle
git checkout nom_de_ma_branch_nouvelle

# Une seule ligne: créer et basculer
git checkout -b nom_de_ma_branch_nouvelle
```

## Supprimer une branch

```shell
# Si la branch est local et n'est pas créée sur le repo distant
git branch -d nom_de_ma_branch_local

# Si la branch est présente sur le repo distant
git push origin --delete nom_de_ma_branch_distante
```

## Changer de branch

```shell

git checkout nom_de_ma_branch

# Ou cela dépend de la vesrion de GIT 
# (donc si vous avez une erreur avec le premier utiliser celui la)

git switch nom_de_ma_branch
```

## Premier commit

```shell
git add .
git commit -m "initial commit"
```

## Commit suivant

```shell
# 'add . ' <= tous les fichier modifier 
# 'add chemin_vers_mon_fichier' <=  pour un fichier cibler

git add chemin_vers_mon_fichier
git commit -m "message du commit"
```

## Annuler le dernier commit et modifs

```shell
git reset --hard md5_commit
git push --force
```

## Mettre à jour le dépôt local

```shell
git pull
```

## Mettre à jour le dépôt local d'une branch spécifique

```shell
git pull origin MA_BRANCH
```

## Crée la branch locale sur GITHUB
```shell
git push --set-upstream origin nom_de_la_branch
# Ou
git push -u origin nom_de_la_branch
```

## Envoyer ses commits vers GITHUB

```shell
git push
```

## Envoyer ses commits vers GITHUB sur une branch spécifique

```shell
git push origin MA_BRANCH
```

## Fusionner une branch avec master

```shell
# On vient ce placer sur Master
git checkout master
# On vient fusionner les fichier (merge)
git merge nom_de_la_branch
# On vient push la fusion des deux 
git push

```
