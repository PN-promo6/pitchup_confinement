# Tutoriel pour le projet Pitchup
Tutoriel pour récupérer et travailler en ligne sur le projet Angular "Pitchup" avec Stackblitz.

## I. Récupérer le projet

### 1. Créer un compte Stackblitz
- Allez sur : [stackblitz.com](https://stackblitz.com/)
- Créez un compte ⚠️ **avec votre compte Github** ⚠️

### 2. Forker le projet "pitchupconfinement"
- Retrouvez le projet sur [stackblitz.com/edit/pitchupconfinement](https://stackblitz.com/edit/pitchupconfinement)
- Cliquez sur "Fork" en haut à droite, pour l'associer à votre compte

### 3. Renommer le fichier
- Renommez le projet en utilisant **le champ en haut à gauche** de la fenêtre : ![Renommer projet](https://i.ibb.co/hygbPBV/Annotation-2020-04-03-114946.png)
 - Utilisez le format de nommage suivant : pitchupconfinement_ *vos initiales*
- Vérifiez que le projet est bien ajouté à votre compte en cliquant sur votre pseudonyme en haut à droite
 - S'il n'est pas là, recommencez ! :)

## II. Créer un component
Pour créer un component, nous passons d'habitude par la console avec la commande `ng g c` , sur Stackblitz, il n'y a pas de terminal nous permettant cela, il faut donc les **créer à la main** en veillant à **n'oublier aucune étape** !

### 1. Récuperer le fichier d'exemple sur le repository [pitchup_confinement](https://github.com/PN-promo6/pitchup_confinement)
- **Renommer** le fichier en remplaçant "Example" par le nom de votre component
- **Modifier** le fichier en remplaçant **toutes les occurrences de "Example"** par le nom de votre component

### 2. Déclarer le component dans `app.modules.ts`
- Déclarer le component en haut du fichier
 - Exemple avec _ExampleComponent_ : `import { ExampleComponent } from './example/example.component';`
- L'ajouter à l'array `declarations` plus bas dans le fichier

**➡️ En cas de doute : prendre exemple sur tous les components déjà créés**
