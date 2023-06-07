# La clean architecture: une solution pour augmenter la maintenabilité de ses systèmes

### Conférencier: Mehdi BOISSAT-BRON

## Intro
- Assurer la maintenabilité
- Facilter le partage de features entre microservices
- Ancticiper des chantiers techniques
Cela résulte en ce choix de clean archi

Représentation:
Entities Domain > Usecases > Handlers/controllers > UI/Systèmes externes
Dependency rule (Dernière couche a connaissance des premières mais pas l'inverse)

## Mise en place
- Définition d'une arborescence
- Domain est accessible
- Centralisation du code métier
- Respect dependency rule
  
## Avantages
Plus maintenable, meilleur coverage des tests
Partage de fonctionnalités facilité par les usecases
Remplacement des composants facilité
Permet de travailler à plusieurs sur une même US

## Inconvenients
Pas applicable à tous les cas (code externe par exemple)
Compliqué à mettre en place sur code legacy
