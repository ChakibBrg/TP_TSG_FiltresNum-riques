# TP2: Filtres numériques

Ce TP vise à concevoir un filtre numérique pour filtrer un signal bruité dont le spectre du signal utile est compris entre les fréquences de coupure de 1 kHz et 3 kHz. Nous utiliserons un filtre RII de type passe-bande.

## 1. Type du filtre
C'est un filtre RII de type passe-bande entre les deux fréquences: 1 kHz et 3 kHz.

## 2. Calcul des fréquences normalisées de ce filtre
Les fréquences de coupure normalisées sont calculées en divisant les fréquences de coupure par la fréquence maximale.


Pour calculer la fréquence maximale, on utilise le théorème de Shannon :  **fréquence_maximale = fréquence_d'échantillonage / 2**

## 3. Trouver les coefficients \( a_i \) et \( b_i \) du filtre RII
Les coefficients du filtre sont calculés à l'aide de la fonction `signal.butter`.

## 4. Trace de la réponse impulsionnelle (avec 50 échantillons)
La réponse impulsionnelle du filtre est tracée à l'aide de la fonction `signal.dimpulse`.

## 5. Trace de la fonction de transfert
La fonction de transfert du filtre est tracée à l'aide de la fonction `signal.freqz`.

## 6. Effet de l'augmentation de l'ordre sur la courbe
L'effet de l'augmentation de l'ordre du filtre sur la courbe est illustré en traçant la fonction de transfert pour différents ordres de filtre. On remarque que l'augmentation de l'ordre du filtre rapproche la réponse du filtre du cas idéal, mais un ordre très élevé peut conduire à des comportements inattendus tels que l'amplification de certaines fréquences ou une atténuation excessive du signal.

## Exécution du code
Le code fourni peut être exécuté dans un environnement Python avec les bibliothèques numpy, matplotlib et scipy installées. Chaque section du code est commentée pour une compréhension claire de chaque étape.

