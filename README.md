# Orion District · Démonstration V5

Trois accès publics sur GitHub Pages :
- Client : https://alpha19-b.github.io/orion-district-demo/client.html
- Administration : https://alpha19-b.github.io/orion-district-demo/administration.html
- Boutique directe : https://alpha19-b.github.io/orion-district-demo/boutique.html

## À essayer
Client → Me connecter → Aïssatou (Premium), ou Mamadou (VIP).
Créer un programme selon son expérience ; réserver un massage ou bilan ; saisir un résultat fictif ; suivre les tendances ; terminer une séance et renseigner l’effort ; ajouter un exercice au carnet ; retrouver la réduction dans la boutique.
Visiteur : ouvrir la boutique sans compte ou créer un compte sans abonnement.
Administration : choisir le rôle admin, manager, réception ou vendeur. Les rendez-vous bien-être et la maintenance sont accessibles aux rôles concernés.

## Fonctionnement de la démonstration
Site statique. Données fictives dans le stockage local du navigateur. Les deux espaces du même navigateur partagent ce stockage ; chaque onglet conserve une session de démonstration séparée par espace. Aucun partage de données entre appareils. Pas de serveur d’authentification : les rôles sont une simulation d’interface, pas une sécurité de production.
Les bilans corporels et exports sont affichés au membre courant uniquement dans l’interface. Ne pas saisir de données personnelles réelles.
Le QR est temporaire et lisible, sa validation est locale. Aucun tourniquet, fauteuil ou analyseur n’est connecté. Aucun paiement réel. Les tarifs de bien-être sont des hypothèses de démonstration à valider par le club.
L’analyse du programme décrit les séances enregistrées, la fréquence et l’effort déclaré. Elle ne fait pas de diagnostic ni de prescription. Les séances de performance sont des cadres à compléter avec un coach.

## Organisation
`client.html` et `administration.html` chargent les mêmes ressources à la racine du dépôt, avec des routes et sessions distinctes. `boutique.html` ouvre directement le catalogue client. L’ancienne adresse racine redirige vers le bon espace en conservant son lien profond.
Publication automatique depuis la branche `main`, racine du dépôt. Aucun outil de compilation requis.

## Inspiration fonctionnelle
[Application Basic-Fit](https://www.basic-fit.com/fr-fr/basic-fit-app) : accès QR, programme, suivi et services du club. Identité visuelle et expérience Orion conservées.
Bibliothèque QR : qrcode-generator, Kazuhiko Arase, licence MIT (notice conservée dans qrcode.js).
