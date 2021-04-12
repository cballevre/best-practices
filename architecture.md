# Architecture

### 1. Limiter le nombre de requêtes HTTP

Mieux découper les responsabilités entre le back et le front

* Client : environnement pas contrôlable (coût en ram lors de traitement)
* Serveur : environnement maitrisé (si pris en compte dans la conception)

Cependant la communication entre les deux consomme de la bande passante et cela à un coup. 

Utilisé la puissance d'HTTP2 : 
- Flux multiplexés
- Server Push

Mettre en place un [cache](./cache.md) surtout pour un api REST 

Question :
- Filtrer les données au niveau du back ou du front 
- 


Source : 
- [Qu’est-ce que le HTTP/2 – Le guide ultime](https://kinsta.com/fr/apprendre/http2/#what_is_http2)



