J'ai eu plusieurs phases dans mon projet de Deep Learning, dernierement réecrit mon projet integralement, voila derniere version en Date, que j'utilise pour faire mes recherche en prediction des time series : https://github.com/VadimKashtanov/Filtres-1.4-4a1c3a1-


# Expériance Optimisation Mathématique #

Mon plus gros projet en optimisation Mathématique est la conception et l'implémentation d'une méthode de Calcule de la Matrice Hessienne pour tout type de Model. La vitesse de cet amgorithme peut etre quasiement égale a celle d'un simple forward-Backward pour obtenire seulement le Gradient des poids du Model. Tout depends de la precision et de la nature du model.

Le probleme était tout autant informatique que mathématique. Car c'est la double dérivation d'une fonction quelconque f0(f1(f2(f3 ... fn(x)))) de maniere stable.

Je n'ai pas fait de version présentable, car je travaille toujours dessus, mais voici le fichier python (pas cuda) "théorie" : https://github.com/VadimKashtanov/fichier_dL_ddL.  Le fichier montrer que l'algorithme donne des résultats exacte et en un temps quasiement n fois plus court que si on fesait une itération de forward-backward.

J'ai implémenté ma méthode en C++/CUDA ici :  https://github.com/VadimKashtanov/V-1.12/ . Il n'y a pas qu'un seul fichier car la méthode implique d'etre implémenté pour tout type d'instruction (couche d'un model).

# Expériance Machine Learning & Deep learning #

J'ai eu plusieurs versions pour mon projet d'IA :
* Une premiere version 100% en C sur CPU qui pouvait resoudre des problemes de XOR a MNIST.
* Une seconde expériance qui est résté une expériance ou je travaille sur la selection naturelle des reseau de neurones non denses.
* Et enfin la version "moderne" qui ressemble probablement a un Tensorflow : https://github.com/VadimKashtanov/Filtres-1.4-4a1c3a1-

Ma lib peut resoudre tout type de problemes. Seulement je me suis concentré depuis 1.5 ans sur la prédiction des "time series" a savoire la prédiction des courbes dans le temps (ex : le cour d'un Marché). J'utilise une methode alternative a LSTM meme si j'ai implémenté une version fonctionnelle et optimisé de LSTM.

Perspectives : Peut etre que je passerai a des problemes plus complexes comme la compehention de la langue, mais je pense que ça fera l'objet de mon Master 2.

# Expériance Data Visualisation #

J'ai beaucoup utilisé matplotlib pour visualiser les données des problemes que j'ai rencontré. Je n'ai pas de projet spécifique, car c'est un outil, tout comme la visualisation elle meme.

# Expériance Calcule Haute performance & Vitesse avec CUDA #

J'ai donc implémenté sans cuBLAS la Convolution, les couches Denses (multiplication de matrice maximalement rapides, avec une somme et un fonction d'activation f(ax+b)) et LSTM/GRU.

De tout maniere tout est dérivé de la multiplication de matrice, j'ai donc fabriqué une librairie ou je peux librement implémenter tout type de couche.
