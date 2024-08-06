# Angular

Angular est un framework open-source développé et maintenu par Google pour la création d'applications web dynamiques. Il est particulièrement apprécié pour sa capacité à créer des applications à page unique (SPA) avec une architecture modulaire. Voici quelques concepts et exemples de base pour t'aider à démarrer :

### Concepts Clés

1. **Components** : Les composants sont les blocs de construction de base d'une application Angular. Chaque composant a une vue associée (HTML) et une logique (TypeScript).

2. **Modules** : Les modules sont des conteneurs pour un groupe de composants, directives, pipes, et services qui sont liés fonctionnellement.

3. **Services** : Les services sont utilisés pour partager des données et des fonctions entre différents composants.

4. **Directives** : Les directives sont des classes qui ajoutent un comportement supplémentaire aux éléments dans vos applications Angular.

5. **Dependency Injection** : Angular utilise l'injection de dépendances pour améliorer la modularité et la réutilisabilité du code.

### Exemple de Création d'une Application Simple

#### Installation d'Angular CLI

Pour commencer avec Angular, tu peux installer Angular CLI (Command Line Interface) en utilisant npm :

```bash
npm install -g @angular/cli
```

#### Création d'une Nouvelle Application

Pour créer une nouvelle application Angular, utilise la commande suivante :

```bash
ng new my-angular-app
cd my-angular-app
ng serve
```

Cette commande crée une nouvelle application et lance un serveur de développement. Tu peux accéder à l'application en naviguant vers `http://localhost:4200` dans ton navigateur.

#### Création d'un Composant

Pour créer un nouveau composant, utilise la commande suivante :

```bash
ng generate component my-component
```

Cela générera quatre fichiers pour le composant :

- `my-component.component.ts` : Logic du composant
- `my-component.component.html` : Template HTML
- `my-component.component.css` : Styles CSS
- `my-component.component.spec.ts` : Tests unitaires

#### Exemple de Composant

Voici un exemple de ce à quoi peut ressembler un composant simple :

**my-component.component.ts**
```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'app-my-component',
  templateUrl: './my-component.component.html',
  styleUrls: ['./my-component.component.css']
})
export class MyComponent {
  title = 'Hello Angular!';
}
```

**my-component.component.html**
```html
<h1>{{ title }}</h1>
```

#### Utilisation du Composant

Pour utiliser ce composant dans ton application, ajoute le sélecteur `<app-my-component>` dans le template principal `app.component.html` :

**app.component.html**
```html
<app-my-component></app-my-component>
```

### Aller Plus Loin

Pour des fonctionnalités plus avancées, comme la gestion des formulaires, la communication avec un backend, ou l'utilisation de services, Angular propose une documentation complète et des tutoriels sur son site officiel : [Angular Documentation](https://angular.io/docs).

Si tu as des questions spécifiques ou un projet en tête, n'hésite pas à me fournir plus de détails pour que je puisse te donner des conseils plus adaptés.
