# WildBlog - Atelier Debug

Bienvenue dans l'atelier de debug ! Ce projet **WildBlog** est le résultat attendu après les quêtes 1 à 9 de ton parcours Angular. Ton objectif ? **Débugger** l'application pour la rendre pleinement fonctionnelle.

> ⚠️ **Note** : Ce projet est fait sous Angular 17, donc certaines fonctionnalités peuvent être spécifiques à cette version.

## Instructions

1. **Installe les dépendances**  
   Lance `npm install` pour installer toutes les dépendances nécessaires.

2. **Lance l’application**  
   Démarre le serveur de développement avec `ng serve` et ouvre l’application sur `http://localhost:4200/`.

3. **Débugge le code**  
   Corrige toutes les erreurs et fais en sorte que l’application fonctionne correctement.

4. **Note tes corrections**  
   Garde une trace des erreurs corrigées pour suivre ta progression.

Bon debug ! 🛠️


# Guide : Cloner un dépôt GitHub et le reconfigurer sur votre propre dépôt

Ce guide décrit les étapes pour cloner un projet existant depuis GitHub, le reconfigurer localement, et manipuler les branches et remotes pour créer un dépôt personnel.

## Étapes

### 1. Cloner le dépôt existant

```bash
git clone https://github.com/WildCodeSchool/angular17_debug_quest.git
cd angular17_debug_quest
```

### 2. Supprimer l'historique Git pour repartir sur un nouveau dépôt

```bash
rm -rf .git
```

### 3. Initialiser un nouveau dépôt Git

```bash
git init
git add .
git commit -m "Initial commit"
```

### 4. Créer un nouveau dépôt sur GitHub

- Allez sur GitHub et créez un nouveau dépôt sans suffixe (par exemple, angular17_debug_quest).
- Copiez l'URL du nouveau dépôt.

### 5. Ajouter le dépôt distant (remote) et pousser les changements

#### A. Ajoutez le dépôt GitHub en tant que remote :
```bash
git remote add origin https://github.com/odowin/angular17_debug_quest.git
```
#### B. Poussez le contenu vers le dépôt distant :
```bash
git push -u origin master
```

# Manipulation des branches

## Créer une nouvelle branche avec un nouveau nom

### 1. Assurez-vous d'être sur la branche de départ (par exemple, master) :

```bash
git checkout master
```

### 2. Créez une nouvelle branche et basculez dessus :

```bash
git checkout -b v0
```

### 3. Poussez cette nouvelle branche vers GitHub :

```bash
git push -u origin v0
```

## En cas d'erreur avec les remotes
Si vous ajoutez un mauvais remote par erreur, vous pouvez le supprimer et en ajouter un nouveau :

### 1. Supprimez le remote existant :

```bash
git remote remove origin
```

### 2. Ajoutez le bon remote :

```bash
git remote add origin https://github.com/odowin/angular17_debug_quest.git
```

## Commandes utiles en résumé

Cloner un dépôt :
```bash
git clone <URL_DÉPÔT>
```
Initialiser un nouveau dépôt :
```bash
git init
```
Ajouter un remote :
```bash
git remote add origin <URL_DÉPÔT>
```
Supprimer un remote :
```bash
git remote remove origin
```
Créer une nouvelle branche :
```bash
git checkout -b <nom_branche>
```
Pousser vers le dépôt distant :
```bash
git push -u origin <nom_branche>
```
