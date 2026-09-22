# HTML — Le modèle mental

**Difficulté :** 🟢 Découverte

HTML décrit le **sens et la structure** d'un document. Il ne sert pas à faire joli : il donne au navigateur une information structurée qu'il peut afficher, indexer et rendre utilisable.

## 1. Un document est un arbre

```text
Document
├── html
│   ├── head
│   │   ├── title
│   │   └── meta
│   └── body
│       ├── header
│       ├── main
│       └── footer
```

Chaque élément peut contenir des enfants. Cette relation parent/enfant sera fondamentale lorsque nous aborderons le DOM.

## 2. Anatomie minimale

```html
<!doctype html>
<html lang="fr">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Mon document</title>
  </head>
  <body>
    <h1>Bonjour</h1>
  </body>
</html>
```

- `<!doctype html>` indique un document HTML moderne.
- `lang` indique la langue principale.
- `meta charset` définit l'encodage.
- `viewport` aide les navigateurs mobiles.
- `title` donne un titre au document.
- `body` contient le contenu de la page.

> 💡 **À comprendre :** HTML décrit une hiérarchie. Avant le CSS, demande-toi quel contenu existe et quelles relations les éléments ont entre eux.

## 3. Attributs

Un attribut apporte une information supplémentaire à un élément.

```html
<a href="https://example.com" target="_blank" rel="noopener">Visiter</a>
```

Ici, `href`, `target` et `rel` modifient le comportement ou le contexte du lien.

## 4. Règle de raisonnement

Pour chaque élément : quel contenu représente-t-il ? Quel élément exprime le mieux ce sens ? Quels attributs sont nécessaires ? Comment un clavier, un lecteur d'écran et un moteur de recherche comprendront-ils cette structure ?

## Erreurs fréquentes
- utiliser des `div` partout ;
- choisir une balise uniquement pour son apparence ;
- oublier la hiérarchie des titres ;
- confondre structure HTML et présentation CSS.
