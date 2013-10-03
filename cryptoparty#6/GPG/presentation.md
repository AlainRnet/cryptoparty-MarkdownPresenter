#GPG

Confidentialité du contenu des échanges par courriel.

![logo GnuPG](/logo-gnupg.png)


!

# PGP / OpenPGP / GPG / GnuPG ????

* PGP: Pretty Good Privacy 
* Phil Zimmermann 1991
* OpenPGP: standard d'Internet RFC 4880
* GPG: Gnu Privacy Guard
    * logiciel libre sous licence GPL
    * g10 Code, société allemande dirigée par Werner Koch
    * 1999: version 1.0.0
    * 2006: version 2.0

!

# Logiciel libre?

* Que fait réellement mon ordinateur, mon téléphone, mon logiciel?
* Mon ordinateur est-il encore mon ami?

Ordinateur rempli de logiciels non-libres:
![boîte noire](/hal.jpg "Ordinateur rempli de logiciels non-libres:")

!

# Logiciels non-libres ou propriétaires

* code source fermé
* mécanisme interne: secret commercial
![poison](poison.jpg)

!

# Logiciel libre

* libre accès au code source
* accès aux mécanismes internes du logiciel, du système d'exploitation

Ordinateur avec du logiciel libre dedans:
![raspberry pi boîtier transparent](boite-transparente.jpg)

!

# Logiciel libre

![gnulinux](/gnu-linux.jpg)

!

# Chiffrement

Classiquement:
![chiffrement symétrique](/symmetric.png)

* 1 seule clef pour chiffrer et déchiffrer
* Chiffrement dit "symétrique"

!

#Chiffrement symétrique

Objectif: chiffrer nos mails

!

#Chiffrement symétrique

Problèmes du chiffrement symétrique:

* Comment envoyer la clef sans se la faire piquer?
* 1 clef différente par couple expéditeur-destinataire, ça fait beaucoup de clefs
![beaucoup de clefs](/clefs.jpg)

!

La solution en vidéo!

!

#Cryptographie à clef publique

* concept 1976 Diffie & Hellman
* mise en pratique en 1978 par
    * **R**ivest
    * **S**hamir
    * **A**dleman
* **RSA** est l'algorithme de chiffrement asymétrique le plus utilisé dans GPG

!

# Que fait GPG ?

* Confidentialité
    * Chiffrement du message
    * Déchiffrement du message
* Signature du message
    * authentification de l'expéditeur
    * intégrité du message
* Création des paires de clefs
* Gestion des clés
* Certification des clefs
* Révocation des clefs compromises

!



!

# Applications de GPG

* Email bien sûr, mais pas que...
* 
*

!

# "The Crypto Wars"

* Zimmermann: activiste pacifiste et antinucléaire
* 1993 Zimmermann devient la cible d'1 enquête criminelle de la part du gouvernement américain
* "Exportation de munitions sans licence"
* crypto avec clef > 40 bits considérée comme munitions
* PGP: clefs de 128 bits (1993)
* publication du code source du programme en version papier! Livre protégé par 1er amendement 
* 1996 enquête fédérale criminelle abandonnée sans mise en examen de Zimmermann
* démilitarisation de la "crypto forte"  = nécessité économique du chiffrement? (banque, e-commerce)

!

...

!

# Serveur de clés

* Comment Alice peut récupérer la clef publique de Bob?
    * Bob envoie sa clef publique à Alice par mail, en pièce jointe
    * Bob transmet sa clef publique à Alice via 1 clef USB
    * Bob dépose sa clef publique sur un serveur de clefs...

!

# Serveur de clés

* sorte d'annuaire
* [https://sks-keyservers.net/](https://sks-keyservers.net/)

!

# Web of Trust

* Toile de confiance
* On ne peut physiquement vérifier qu'un nombre limité de clés
* Signature des clés

