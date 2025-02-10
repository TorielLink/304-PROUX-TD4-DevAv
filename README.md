# TD4 Développement avancé
## Question 1.1
La taille par défaut d'une clef RSA est de 2048 bit. Pour l'augmenter à 4096 bits, il faut tapper la commande : `openssl genpkey -algorithm RSA -out private_key.pem -pkeyopt rsa_keygen_bits:4096
`.