# HTML — Liens et médias

**Difficulté :** 🟡 Application

## Liens

```html
<a href="/contact">Me contacter</a>
<a href="https://example.com">Site externe</a>
<a href="#competences">Voir mes compétences</a>
```

Distingue chemin absolu, chemin relatif et fragment. Un lien doit avoir un texte compréhensible hors contexte immédiat.

## Images

```html
<img src="/images/profil.webp" alt="Portrait devant un ordinateur">
```

`alt` décrit l'information utile. Une image décorative peut avoir `alt=""`.

## Vidéo

```html
<video controls preload="metadata">
  <source src="/media/demo.mp4" type="video/mp4">
  Votre navigateur ne peut pas lire cette vidéo.
</video>
```

Pour chaque média : est-il nécessaire ? quelle information porte-t-il ? que se passe-t-il s'il ne se charge pas ? faut-il une alternative ?
