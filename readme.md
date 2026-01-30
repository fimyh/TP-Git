# Durée

## Pourquoi utiliser Git ?

Git est un outil de gestion de versions.

Il permet de :

- garder l’historique des modifications
- revenir à une version précédente
- travailler à plusieurs sur un même projet
- sécuriser son code

👉 Git est utilisé dans presque tous les projets informatiques (développement, QA, data…).

## Git vs GitHub / GitLab

**Git** :

- outil installé sur l’ordinateur
- fonctionne en local
- ne nécessite pas Internet

**GitHub / GitLab** :

- plateformes en ligne
- permettent de partager le code
- facilitent le travail en équipe

📌 GitHub ≠ Git

## Concepts clés de Git

- **Dépôt (repository)** : dossier suivi par Git
- **Fichier non suivi** : fichier inconnu de Git
- **Fichier suivi** : fichier pris en compte par Git
- **Zone de staging** : zone de préparation
- **Commit** : sauvegarde de l’état du projet
- **Branche** : ligne de travail parallèle

## Installation et configuration

**Installation**

- Télécharger Git
- Vérifier l’installation :

```
git --version
```

**Configuration minimale**
```
git config --global user.name "Nom"
git config --global user.email "email@test.com"
```

## Créer un premier dépôt Git

Se placer dans le dossier du projet puis :

```
git init
```

Vérifier l’état du dépôt :

```
git status
```

## Enregistrer des modifications

**Workflow de base**
```
git add .
git commit -m "Message de commit clair"
```

- `git add` : prépare les fichiers
- `git commit` : enregistre une version

📌 Bonne pratique :  
1 commit = 1 modification logique

## Consulter l’historique

Voir l’historique des commits :

```
git log
```

Voir les différences entre versions :

```
git diff
```

## Annuler une erreur simple

Git permet de :

- annuler une modification non validée
- corriger un message de commit
- revenir à une version précédente

👉 En pratique, presque toutes les erreurs sont récupérables.

## Les branches (version simplifiée)

La branche principale s’appelle `main`.

Une branche permet de travailler sans impacter le code principal.

Très utilisée pour :

- nouvelles fonctionnalités
- tests
- corrections

Créer et utiliser une branche :

```
git checkout -b nouvelle-branche
```

## Fusionner une branche

Revenir sur la branche principale :

```
git checkout main
```

Fusionner :

```
git merge nouvelle-branche
```

📌 Un conflit peut apparaître, ce n’est pas une erreur.

## Git et les dépôts distants

**Dépôt distant**

- Hébergé sur GitHub / GitLab
- Sauvegarde du projet en ligne

**Commandes essentielles**
```
git clone
git push
git pull
```

- `clone` : copier un projet existant
- `push` : envoyer les modifications
- `pull` : récupérer les modifications

## Workflow simple recommandé

- Modifier les fichiers
- Vérifier l’état
```
git status
```

- Ajouter les fichiers
```
git add .
```

- Créer un commit
```
git commit -m "message"
```

- Envoyer sur le dépôt distant
```
git push
```

## Erreurs courantes à éviter

- Oublier de faire des commits
- Faire des commits trop gros
- Messages de commit peu clairs
- Avoir peur de Git 😄

💡 Git est un outil sûr et tolérant.

## Exercice pratique (30–45 min)

- Créer un dépôt local
- Ajouter un fichier texte
- Faire 2 commits
- Créer une branche
- Modifier un fichier
- Fusionner la branche
- Envoyer le projet sur GitHub / GitLab

## Conclusion

Git est indispensable aujourd’hui.

Les commandes de base suffisent largement.

La pratique est essentielle.

## Ressources utiles :

- Git Cheat Sheet
- Documentation officielle Git
- Exercices en ligne