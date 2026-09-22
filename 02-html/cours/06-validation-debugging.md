# HTML — Validation et debugging

**Difficulté :** 🟡 Application → 🟠 Autonomie

Après une première implémentation, cherche d'abord à **reproduire** le problème.

## Méthode

```text
Symptôme → Reproduction → Hypothèses → Test ciblé → Cause → Correction → Régression
```

## Séparer les couches

- **Structure :** le bon élément existe-t-il ?
- **Contenu :** le texte ou la donnée est-il correct ?
- **Présentation :** le CSS modifie-t-il l'affichage ?
- **Comportement :** JavaScript intervient-il ?

> ✅ **À retenir :** corrige la cause, puis vérifie qu'aucune régression n'est apparue.
