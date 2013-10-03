#Plan cryptoparty

* Titre

* Présentation (but + nous ?)
   * But de la cryptoparty

* Vocabulaire
   * Algorithme ? Code source ? Binaire ?
      * Algorithme  : recette de cuisine, lisible par un humain
      * Code source : ingrédients lisible par un humain
      * Binaire     : plat finalisé, lisible par une machine, on ne peut pas
                      revenir au code source
   * Logiciel libre
      * Code source accessible
      * Liberté de redistribuer, modifier, distribuer la version modifiée, vendre
      * Avantage en sécurité : comme tout est accessible on sait que cela fait ce
        pourquoi il est vendu

   * Cryptographie ? Cryptoanalyse ? Cryptologie ?
      * Cryptographie : Création d'algorithme spécialisé pour le chiffrement (issu
        directement des théories mathématiques)
      * Cryptoanalyse : Analyse mathématique diverse dans le but de casser un
        algorithme de chiffrement (trouver des failles, faiblesses, qui fragilisent
        l'algo pour le rendre inutile)
      * Cryptologie   : La science qui rassemble la cryptographie et la cryptoanalyse

   * Chiffrer, déchiffrer, décrypter (encrypter n'existe pas)
      * Chiffrer   : passer de données en clair à un chiffre a l'aide d'une clé
      * Déchiffrer : passer d'un chiffre à des données en clair à l'aide d'une clé
                     connue
      * Décrypter  : Déchiffrer des données sans connaitre la clé initialement
                     (casser un chiffre)
      * Crypter, encrypter : n'existe pas

   * Alice, Bob, Eve
      * Alice et Bob cherchent à communiquer, Eve cherche à espionner/casser

   * Chiffrement sym/asym

* Pessimisme
   * On est pas anonyme sur internet (on ne peux pas être totalement, que partiellement)
   * On est pas protégé contre l'écoute
      * Corollaire : on est pas protégé contre la rétention
   * On ne PEUT PAS étre protégé à vie
   * Il n'y a pas de sécurité sans apprentisage

* Dafuq is internet ?
   * Réseau standardisé regroupant d'autres réseaux
   * Le paquet IP :
       --------------
      | OH | Payload |
       --------------
   * Les traces :
      * "votre" routeur
      * votre FAI
      * tout serveur entre les deux
      * le serveur destinataire

* SSL (https)
   * SSL chiffre uniquement le payload
   * un observateur extérieur ne voit pas les données utiles, mais voit quelles IP
     communiquent entre elles

* Tor
   * explication de Tor (réseau interne, serveur de sortie, hidden service)
   * au sein du réseau : OH et payload chiffrés
   * aprés le noeud de sortie : RIEN de chiffré

* Mail
   * Protocol distribué (client, et plein de serveurs qui discutent entre eux)
   * Mail copié des dizaines et des dizaines de fois

* GPG
   * 

* Y'a t'il un espoir ?
   * Que faire contre l'écoute massive ?
      * La NSA possède un datacenter capable de retenir 100 ans de données d'appel
        et mails
      * Le Royaume-Uni bosse avec la NSA
      * La France écoute au niveaux des frontières
      * L'Allemagne fait passer des lois pour l'écoute et la rétention
      * Que font les autres pays ?
   * Éviter d'utiliser des services dans des pays connus
   * Tout chiffrer
   * Considérer que dans 5 à 10 ans, ce qui est chiffré aujourd'hui sera cassé
     (donc si ça a été enregistré, ça sera cassé)
