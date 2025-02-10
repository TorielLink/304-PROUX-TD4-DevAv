# TD4 Développement avancé
## Question 1.1
La taille par défaut d'une clef RSA est de 2048 bit. Pour l'augmenter à 4096 bits, il faut tapper la commande : `openssl genpkey -algorithm RSA -out private_key.pem -pkeyopt rsa_keygen_bits:4096
`.

## Question 1.2
Pour extraire la clef publique, on utilise la commande : ``openssl rsa -in server.key -pubout -out server.pub
``.

## Question 2.1
La commande pour générer une nouvelle paire de clef RSA protégé avec l'algorithme DES3 est : ``openssl genrsa -out server.key -des3`` (avec le mot de passe 'toto').

## Question 2.2
La clef publique est chiffrée.

## Question 3.1
Condensat de mon fichier index.js :
- avec sha256 : ``SHA256(index.js)= 96b56c2fbd7700af3f83365398c7bd3c18c50648aa016cbc4f66d3f11fc28bbd``
- avec md5 : ``MD5(index.js)= d86c84d128b3c69c24bed2601cacdb36``
- avec sha-1 : ``SHA1(index.js)= 4ee8335d21d3c7f401d36b4f8624c8e6e6f770dd``

## Question 3.2
``openssl dgst -sha256 -verify server.pub -signature index.js.sign index.js
``