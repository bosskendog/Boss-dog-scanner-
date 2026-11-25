BOSS DOG SCANNER — AJOUT DE L'IA

Dans le dépôt GitHub existant, remplace le fichier index.html par celui fourni ici.
Ajoute le dossier netlify à la racine du dépôt, avec le fichier:
netlify/functions/analyze.mjs

Ne publie JAMAIS ta clé API dans GitHub. Elle doit rester dans Netlify sous:
OPENAI_API_KEY
avec la portée Functions.

Après le commit, Netlify doit redéployer le site. Si nécessaire, lance un nouveau deploy depuis Netlify.

L'analyse d'image utilise l'API OpenAI Responses avec le modèle gpt-4.1-mini. Les appels API sont facturés séparément de ChatGPT.
Les données des fiches restent dans le stockage local du navigateur sur cet appareil; elles ne sont pas synchronisées entre appareils.
