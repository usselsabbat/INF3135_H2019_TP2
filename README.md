# INF3135_H2019_TP2
Travail pratique #2 modification d'un programme/logiciel

### Tous les requis du TP1 doivent être réparé
 + le fichier Makefile doit etre present et fonctionnel; 
 + le fichier `cp.txt` doit contenir votre code permanenent doit être présent à la racine;
 +

### Toutes les informations devront être ajoutées au `wiki` et les questions à la section `issues`
 + aucune question par courriel, toutes les questions devront être posées dans le gestionnaire de version;
 + vous pouvez guider vos collègues avec des réponses; maximum 5 interventions;
 + la qualité des interventions sera notée;
 + la qualité du francais sera aussi notée;
 + les questions sont pour l'obtention de précision uniquement;
 + si une question vise un élement académique incompri, nous adresserons celui-ci en classe;
 + aucune demande de solution ne sera tolérée.

### Vous devez obligatoirement ajouter à votre programme les élements suivants :
#### Vous devez,
+ utiliser des entiers 128bit;
+ ajouter une option `-d ASC | DEC` à la ligne de commande, le default est DEC;
+ utiliser l'instruction `struct` nommé `element` pour maintenir les nombres parfaits trouvés;
+ définir un ou plusieurs `typedef`;
+ définir toutes vos fonctions dans un fichier nommé `outils.h`
+ inclure le fichier `temps.h`;
+ inclure le fichier 'array.h` ou `btree.h`;
+ fournir des informations d'exécution dans la sortie d'erreur `stderr` lorsque le symbole TEMPS est défini;
+ utiliser une ou plusieurs fois la fonction `malloc()`;
+ utiliser une ou plusieurs fois le _keyword_ `enum`;

### Detection des fuites de memoire
+ Vous devez soumettre votre programme à `valgrind`


### Vous devez avoir votre propre projet dans votre gestionnaire de version préféré :
+ le fuseau horaire doit être correctement configuré;
+ le nom du projet doit être en minustcule et sans faute;
+ les utilisateurs de GitLab doivent s'assurer que la sécurité soit adéquate;
+ vous n'avez pas à créer de répertoire pour ce travail;


# Barème de correction

| Critère | Sous-critère | Points |
| ------- |:------------ | ------:|
| Fonctionnabilité  | 5 à 10 tests seront lancés (comparaison binaire) | 6.0 |
| Compilation       | sans avertissement ni erreur                     | 1.0 |
| Git clone         | récupération (droit lecture, écriture)           | 1.0 |
| Qualité           | temps d'exécution (performance) et code          | 2.0 |
| Directives        | création de code.txt                             | 0.5 |
| Makefile          | <ul><li>make</li><li>make clean</li><li>make data</li><li>make test</li><li>make resultat</li></ul> | <ul><li>1.0</li><li>0.5</li><li>1.0</li><li>0.5</li><li>0.5</li></ul> |
| Markdown          | README.md                                        | 1.0 |
| **Total**         |                                                  |  15 |
