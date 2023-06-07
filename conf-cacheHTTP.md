# #RetourAuxSources: Le cache HTTP

### Conférencier: Hubert Sablonnière

## Avantages

- Réduire le chargement client
- Réduicre charge serveur
- Meilleures perfs

max-age du cache définissant le temps de validité de la data
if-modified: 304 si identique, 200 si changement
no-cache --> revalide le cache à chaque fois
no-store --> pas de cache
must-revalidate --> pas de démo :D
immutable --> pas de revalidation en cas de refresh (pas dispo sur chrome car comportement par défaut)
empreinte dans le nom de fichier pour contourner le immutable en cas de changement
possible de rendre un cache private
s-maxage pour un cache partagé avec CDN
accept-language pour cacher sur une langue
vary pour compresser
memory cache VS disk cache
back/forward cache utilisé avec flèches de navigation (congeler notre page)