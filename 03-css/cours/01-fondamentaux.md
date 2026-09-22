# CSS — Fondamentaux

## Objectifs

À la fin de ce module, tu dois pouvoir expliquer et utiliser :

- la cascade ;
- les sélecteurs ;
- l'héritage ;
- la spécificité ;
- le box model ;
- Flexbox ;
- Grid ;
- le responsive design.

## Le bon modèle mental

CSS n'est pas une collection de propriétés à mémoriser.

Le navigateur doit répondre à plusieurs questions :

1. Quels éléments sont concernés ?
2. Quelles règles CSS peuvent s'appliquer ?
3. Quelle règle gagne la cascade ?
4. Quelle taille chaque boîte doit-elle avoir ?
5. Comment les boîtes sont-elles positionnées ?
6. Que se passe-t-il lorsque l'espace disponible change ?

## Cascade

Une règle CSS associe un sélecteur à des déclarations :

```css
.card {
  padding: 1rem;
  border: 1px solid #ddd;
}
```

Lorsqu'une propriété est définie plusieurs fois, le navigateur applique les règles de la cascade, notamment selon l'importance, la spécificité et l'ordre des déclarations.

## Sélecteurs

Exemples :

```css
p {}
.card {}
.card p {}
.card > p {}
input[type="email"] {}
button:hover {}
```

Commence par le sélecteur le plus simple qui exprime correctement l'intention.

## Héritage

Certaines propriétés sont naturellement héritées par les descendants, notamment plusieurs propriétés typographiques.

Ne suppose jamais que toutes les propriétés sont héritées.

## Box model

Un élément peut être représenté comme :

```
margin
┌─────────────────────┐
│ border              │
│  ┌───────────────┐  │
│  │ padding       │  │
│  │  content      │  │
│  └───────────────┘  │
└─────────────────────┘
```

Avec `box-sizing: border-box`, la dimension déclarée inclut le padding et la bordure.

## Flexbox

Flexbox organise principalement les éléments selon une dimension.

Questions à se poser :

- quel est l'axe principal ?
- comment distribuer l'espace ?
- comment aligner les éléments ?
- faut-il autoriser le retour à la ligne ?

## Grid

Grid est particulièrement adapté lorsque la structure nécessite simultanément lignes et colonnes.

## Responsive design

Une interface responsive ne signifie pas seulement « mobile puis desktop ».

Elle doit répondre aux contraintes réelles :

- largeur disponible ;
- lisibilité ;
- densité ;
- taille des contrôles ;
- images ;
- navigation ;
- ordre du contenu.

## Erreurs fréquentes

- utiliser `!important` pour masquer un problème de cascade ;
- utiliser des positions absolues pour construire toute une page ;
- multiplier les breakpoints sans raison ;
- fixer des largeurs qui provoquent de l'overflow ;
- modifier plusieurs variables pendant un debugging.

## Méthode de travail

```
Besoin
  ↓
Structure HTML
  ↓
Layout
  ↓
Espacement
  ↓
Typographie / couleurs
  ↓
États interactifs
  ↓
Responsive
  ↓
Accessibilité
  ↓
Tests
```

## À retenir

Le CSS devient beaucoup plus simple lorsque tu raisonnes en **règles, contraintes, boîtes et contextes de layout**, plutôt qu'en propriétés isolées.
