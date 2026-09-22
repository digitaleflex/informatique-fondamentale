# HTML — Formulaires

**Difficulté :** 🟡 Application

Un formulaire transforme une intention utilisateur en données structurées.

```html
<form action="/contact" method="post">
  <label for="email">Adresse e-mail</label>
  <input id="email" name="email" type="email" autocomplete="email" required>
  <label for="message">Message</label>
  <textarea id="message" name="message" rows="6" required></textarea>
  <button type="submit">Envoyer</button>
</form>
```

- `label` associe une consigne à un champ ;
- `id` permet notamment cette association ;
- `name` identifie la donnée envoyée ;
- `type` exprime la nature attendue ;
- `required` impose une contrainte native ;
- `autocomplete` améliore l'expérience.

## Validation HTML ≠ validation métier

Le navigateur effectue des vérifications utiles, mais le serveur doit considérer les données reçues comme non fiables et appliquer ses propres règles.

> ❌ **Erreur fréquente :** croire que `required` protège à lui seul une application.

Ne remplace pas une étiquette par un simple placeholder : le placeholder est une aide temporaire, le label décrit le champ.
