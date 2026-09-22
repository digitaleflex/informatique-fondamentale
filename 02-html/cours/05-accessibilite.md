# HTML — Accessibilité de base

**Difficulté :** 🟡 Application

## Principes pratiques

1. Utiliser les éléments natifs avant de recréer leur comportement.
2. Donner un nom accessible aux contrôles.
3. Associer les labels aux champs.
4. Respecter une hiérarchie logique des titres.
5. Fournir des alternatives aux images informatives.
6. Ne pas transmettre une information uniquement par la couleur.
7. Vérifier l'utilisation au clavier.

## HTML natif avant ARIA

Un bouton doit généralement être un `button`, pas un `div` avec un clic JavaScript.

```html
<button type="button">Ouvrir le menu</button>
```

ARIA complète la sémantique lorsque le HTML natif ne suffit pas. Elle ne doit pas masquer une mauvaise structure.

## Test clavier

Sans souris : atteindre les contrôles avec Tab, comprendre le focus, activer les actions au clavier et vérifier l'ordre de parcours.
