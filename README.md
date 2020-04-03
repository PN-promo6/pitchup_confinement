# Tutoriel pour travailler en ligne sur le projet Pitchup
Tutoriel pour récupérer et travailler en ligne sur le projet Angular "Pitchup" avec Stackblitz.

## I. Récupérer le projet

### 1. Créer un compte Stackblitz
- Aller sur : [stackblitz.com](https://stackblitz.com/)
- Créer un compte ⚠️ **avec votre compte Github** ⚠️

### 2. Forker le projet "pitchupconfinement"
- Retrouver le projet sur [stackblitz.com/edit/pitchupconfinement](https://stackblitz.com/edit/pitchupconfinement)
- Cliquer sur "Fork" en haut à droite, pour l'associer à votre compte

### 3. Renommer le fichier
- Renommer le projet en utilisant **le champ en haut à gauche** de la fenêtre :
![Renommer projet](https://i.ibb.co/hygbPBV/Annotation-2020-04-03-114946.png)
 - Utiliser le format de nommage suivant : pitchupconfinement_ *vos initiales*
- Vérifier que le projet est bien ajouté à votre compte en cliquant sur votre pseudonyme en haut à droite
 - S'il n'est pas là, recommencer ! :)

## II. Créer un component
Pour créer un component, nous passons d'habitude par la console avec la commande `ng g c` , sur Stackblitz, il n'y a pas de terminal nous permettant cela, il faut donc les **créer à la main** en veillant à **n'oublier aucune étape** !

### 1. Récuperer le dossier d'exemple sur le repository [pitchup_confinement](https://github.com/PN-promo6/pitchup_confinement)
- Récupérer le dossier `example` contenu dans `src/app/`
- Le copier dans `src/app/` sur votre projet
- **Renommer le dossier et ses fichiers** en remplaçant `example` par le nom de votre component
- **Modifier** le fichier `example.component.ts` en remplaçant **toutes les occurrences de `example`** par le nom de votre component :
  - Dans l'objet `@Component({...})`
  - Dans le nom de la classe `export class ExampleComponent`

### 2. Déclarer le component dans `app.modules.ts`
- Déclarer le component en haut du fichier
  - Exemple avec _ExampleComponent_ : `import { ExampleComponent } from './example/example.component';`
- L'ajouter à l'array `declarations` plus bas dans le fichier

### 3. Tester le nouveau component
- Insérer la balise `<app-example><app-example>` (où `example` est le nom de votre component) dans `index.component.html`
- Vous devez voir s'afficher *example works!* sur la page d'accueil du projet

**➡️ En cas de doute : prendre exemple sur tous les components déjà créés**
