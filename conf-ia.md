# D'un modèle d'IA dans un notebook à un service temps réel: architecturons !

### Conférencier: Marie-Alice Blete

## Cycle de vie d'un modèle d'IA
Entrainement --> données utilisées pour créer un modèle
Inférence --> nouvelle donnée passée dans le modèle pour obtenir une prediction (Cas detection de fraude ici)
Modèle entrainé et sérialisé qui devrait être packagé dans un webservice(MasS), le webservice doit s'adapter à différents modèles

# Evolution
Mettre en place l'API connectée au modèle, utiliser un contrat d'interface 
Créer une queue en sortie d'API et passer au compte goutte à l'event processor quand libre (Queue d'attente pour le retour également)
Contrainte de débit et de latence, pour fix le débit il faut faire de la scalabilité, pour la latence on peut mettre en place un TO.
Dépendant du modèle donc concertation entre dev et data scientists
Notre preprocessing réalisé dans le wrapper, rajout de la BDD pour les transactions en entrée

## Resume
Architecture comme une autre malgré ML/IA

## Questions
Onyx envisagé pour changer/accélerer l'inférence
Réentrainer le modèle car les fraudes évoluent pour que cela continue de marcher
Changer totalement d'algo puisque R&D mais peu en prod, discussion avec équipe prod si algo mieux que le précédent