# TD4 Développement avancé
## Question 1.1
La taille par défaut d'une clef RSA est de 2048 bit. Pour l'augmenter à 4096 bits, il faut tapper la commande : `openssl genpkey -algorithm RSA -out private_key.pem -pkeyopt rsa_keygen_bits:4096
`.

## Question 1.2
Pour extraire la clef publique, on utilise la commande : ``openssl rsa -in server.key -pubout -out server.pub
``.
