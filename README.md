# N8N
Créer un bot télégram capable de consulter consulter le google document et d’afficher un message récapitulatif lorsqu’il est appelé avec un petit message bien rédigé. Le bot devra s’appeler Docteur Digiconseil
# n8n - Workflow d'automatisation

## Objectif
- Réception de données médecin via webhook
- Génération d'un Google Doc avec ses infos
- Partage du document Google
- Envoi du lien via Telegram Bot

## Nœuds clés
1. Webhook : réception POST depuis Appsmith
2. Google Drive : création d'un fichier texte avec {{ $json.nom }} etc.
3. Google Drive : partage en lecture seule
4. Telegram : message contenant le lien du fichier

## Tests
- Tester Webhook avec Appsmith (url de production)
- Valider création de fichier dans Google Drive
