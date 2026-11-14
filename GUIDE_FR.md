# Guide de publication sur GitHub (Ubuntu / WSL)

Ce guide suppose que tu as téléchargé le ZIP du projet puis extrait le dossier `power-bi-sales-performance-dashboard`.

## 1. Aller dans le dossier du projet

Adapte le chemin si tu as extrait le dossier ailleurs :

```bash
cd /mnt/c/Users/Marouen/Downloads/power-bi-sales-performance-dashboard
ls -la
```

Tu dois voir `README.md`, `SECURITY.md`, `GUIDE_FR.md` et `report/`.

## 2. Initialiser Git et vérifier les fichiers

```bash
git init
git branch -M main
git add README.md SECURITY.md GUIDE_FR.md .gitignore report/ProjetBI.pbix
git status
```

Vérifie attentivement la liste des fichiers ajoutés. Ne fais pas `git add .` depuis ton dossier personnel (`~`).

## 3. Créer le commit

```bash
git commit -m "Add Power BI sales performance dashboard"
```

## 4. Créer le dépôt sur GitHub

Sur GitHub, crée un nouveau dépôt nommé :

`power-bi-sales-performance-dashboard`

Pour éviter un conflit au premier push, crée-le vide : ne coche pas l'ajout automatique d'un README, d'un `.gitignore` ou d'une licence.

## 5. Envoyer avec SSH

Si ta clé SSH fonctionne déjà avec GitHub :

```bash
ssh -T git@github.com
```

Puis configure le dépôt distant (remplace `TON_UTILISATEUR` par ton identifiant GitHub) :

```bash
git remote add origin git@github.com:TON_UTILISATEUR/power-bi-sales-performance-dashboard.git
git push -u origin main
```

Si `origin` existe déjà, utilise plutôt :

```bash
git remote set-url origin git@github.com:TON_UTILISATEUR/power-bi-sales-performance-dashboard.git
git push -u origin main
```

## 6. Avant de rendre le dépôt public

Lis `SECURITY.md`. Le fichier PBIX contient un modèle de données intégré : vérifie dans Power BI Desktop la source et les données réelles avant de rendre le dépôt public. Si tu n'es pas certain des droits de redistribution ou de l'absence de données sensibles, laisse le dépôt en **Private**.
