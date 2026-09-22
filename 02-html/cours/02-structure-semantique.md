# HTML — Structure sémantique

**Difficulté :** 🟢 Découverte → 🟡 Application

La sémantique consiste à choisir des éléments qui décrivent le **rôle** du contenu.

| Élément | Rôle typique |
|---|---|
| `header` | introduction d'une page ou section |
| `nav` | liens de navigation |
| `main` | contenu principal unique |
| `section` | groupe thématique |
| `article` | contenu autonome |
| `aside` | contenu complémentaire |
| `footer` | informations de fin |

## Exemple

```html
<body>
  <header>
    <a href="/">Mon portfolio</a>
    <nav aria-label="Navigation principale">
      <a href="/projets">Projets</a>
      <a href="/contact">Contact</a>
    </nav>
  </header>
  <main>
    <section aria-labelledby="projets-title">
      <h1 id="projets-title">Mes projets</h1>
      <article>
        <h2>Projet A</h2>
        <p>Description du projet.</p>
      </article>
    </section>
  </main>
  <footer>© 2026</footer>
</body>
```

## Titres : une hiérarchie, pas une taille

`h1` à `h6` décrivent une hiérarchie. Leur choix ne dépend pas de la taille visuelle : le CSS détermine l'apparence.

> ⚠️ **Attention :** ne choisis pas `h4` parce que tu veux un titre plus petit.

## Quand utiliser `div` ?

`div` est un conteneur générique sans signification particulière. Utilise-le lorsqu'aucun élément sémantique ne correspond au besoin.
