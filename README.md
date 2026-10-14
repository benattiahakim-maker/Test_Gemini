# Gemini Dev Test — TaskBoard

Projet de test pour évaluer Gemini 3.8 Flash dans Antigravity.

## Mission

Créer une application web de gestion de tâches en français, en HTML, CSS et JavaScript natifs, sans dépendances ni serveur obligatoire. Elle doit fonctionner en ouvrant index.html.

## Critères d'acceptation

- Ajouter une tâche avec un titre obligatoire (espaces supprimés, 120 caractères maximum), une priorité et une date limite facultative.
- Modifier, terminer, réactiver et supprimer une tâche avec confirmation.
- Filtrer par état et priorité, rechercher dans les titres et trier par date limite (sans date à la fin).
- Afficher les compteurs total, en cours et terminées.
- Conserver les tâches dans localStorage après rechargement et gérer des données de stockage invalides sans bloquer l'application.
- Exporter les tâches en JSON et importer un fichier JSON validé, sans écraser les données en cas d'erreur. Documenter le format choisi.
- Afficher les titres comme du texte : un titre contenant du HTML ne doit jamais exécuter de script.
- Interface responsive, utilisable au clavier, champs étiquetés, messages d'erreur visibles et état vide utile.
- Fournir des tests automatiques pertinents pour validation, filtres, tri et import, exécutables avec Node.js sans dépendances.

## Évaluation manuelle

1. Ajouter trois tâches de priorités et dates différentes ; vérifier les compteurs.
2. Modifier une tâche, la terminer, filtrer puis la réactiver.
3. Recharger la page et vérifier la persistance.
4. Exporter puis réimporter ; vérifier le comportement documenté des doublons.
5. Importer un JSON invalide : message d'erreur et tâches existantes conservées.
6. Ajouter `<img src=x onerror=alert(1)>` : texte affiché, aucune exécution.
7. Tester au clavier et sur une largeur de 375 px.

## Livraison attendue

Code, tests, instructions d'exécution et résumé des vérifications réellement effectuées.