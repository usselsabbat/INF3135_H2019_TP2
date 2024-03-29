# Travail pratique 2 modification d'un programme/logiciel

## Objectifs
  L'objectif est de vous initier à la programmation avec le langage C, en  manipulant
  des données, des fichiers, ainsi que la gestion des `arguments` et `options` provenant de la ligne de commande.

  De plus, vos sources seront maintenues dans un gestionnaire de version/source de type git.

  Vous allez aussi vous familiariser avec `make` et le fichier `Makefile` afin `d'automatiser` plusieurs tâches utiles.

  Dans le `TP2`, nous ajoutons une composante essentielle, les tests. Automatisé des tâches répétitives est quelque chose qui
  reviendra souvent.  Avoir les bons réflexes et la bonne stratégie afin de résoudre un problème, vous garantira à coup sûr
  des résultats à la hauteur de vos attentes.
  
  Préalablement au tests, vous allez modifier votre programme pour devienne sans faille.  La compilation 
  conditionnelle sera expérimenté dans ce travail.  Avec celle-ci il sera possible d'activer ou pas la production de traces.

## Description du travail

  Le programme doit découvrir de nouveaux `nombres parfaits` contenus dans un intervalle composé d’entiers naturels.
  ```math
   N = { 0, 1, 2, ... }
  ```
  Un nombre est dit parfait lorsque la somme des tous ses diviseurs (excluant lui-même bien sûr) est égal à lui-même.

## Qualité du livrable

### Livrer un logiciel parfait est exigé, nous allons donc mettre un peu plus de temps afin de mieux comprendre et livrer un produit de grande qualité.

 + toutes les fonctionnalités du `TP1` doivent être présentes et réparées;
 + le fichier `Makefile` doit être présent et fonctionnel;
 + le fichier `cp.txt` doit contenir votre code permanent doit être présent à la racine de votre projet;
 + aucune librairie non standard; `getopt.h` n'est pas accepté;
 + le fichier `tp2.c` doit contenir uniquement la fonction main();
 + un fichier `outils.h` et un fichier `outils.c` doit exister et contenir les fonctions nécessaire à votre programme;
 + tous les fichiers devront être dans un format `UNIX`.
 
## Exécution et performance
> > + Tous les tests auront une limite de temps;
> > + Chaque exécution ne pourra depasser au maximum 99 secondes;
> > + Il est aussi possible qu'un test soit limité à 10 sec.

## Automatisation des tests unitaire et de regression
 + Tous les tests contenus dans le fichier `inf3135-h2019-tp1.correction` maintenant `inf3135-h2019-tp2.correction` doivent être exécutés sans problème par le script `evaluer.sh`;
 + Il existe plusieurs façons de faire les tests. Nous utilisons le `bash` dans ce travail;
 + Vous devez produire quelque chose de similaire à `output`.

#### output
~~~~
0 : echec
1 : reussi 1 pts
2 : reussi 1 pts
3 : reussi 1 pts
4 : reussi 1 pts
5 : echec
6 : reussi 1 pts
7 : reussi 2 pts
8 : reussi 2 pts
9 : echec
10 : reussi 1 pts
11 : echec
12 : echec
13 : reussi 1 pts
14 : echec
15 : echec
16 : echec
17 : echec
18 : echec
19 : echec
20 : echec
21 : echec
22 : echec
23 : echec
Note (total) pour FRAG01010199 dans inf3135-h2019-tp2: 11
FIN.
~~~~

> > Voici la variante que je propose pour le tp2 (simplifié et légèrement plus facile à travailler) :
> > 
> > [inf3135-h2019-tp2.correction](https://github.com/guyfrancoeur/INF3135_H2019_TP2/blob/master/inf3135-h2019-tp2.correction)
> > 
> > #### colonnes
> > + 1 : points
> > + 2 : temps maximum d'exécution
> > + 3 : code de retour
> > + 4 : description
> > + 5 : commande
> > 
> > Idéalement vous devez ouvrir ce fichier et consommer les données contenues pour parvenir à tester votre programme de façon automatisé.
> > 
> > **Un exemple**
> > 
> > ```bash
> > #!/bin/bash
> > # evaluer.sh
> > wget -q https://github.com/guyfrancoeur/INF3135_H2019_TP2/raw/master/inf3135-h2019-tp2.correction -O inf3135-h2019-tp2.correction
> > if [ ! -f inf3135-h2019-tp2.correction ]
> > then
> >   exit 1
> > else
> >   #echo "fichier OK (garder cette ligne durant le developpement (enlever lors de la remise ou la production)"
> > fi
> > # on continue avec le reste du code ...
> > ```


## Exigences spécifiques
 + tous compléments d'informations seront ajoutées au `wiki`;
 + toutes les questions seront ajoutées à la section `issues`;
 + aucune question par courriel;
 + toutes les questions devront être posées dans le bon fils (sujet pertinent);
 + vous pouvez guider vos collègues avec des réponses; maximum 3 interventions (questions ou réponses);
 + la qualité des interventions sera notée;
 + la qualité du français sera aussi notée;
 + les questions sont pour l'obtention de précision uniquement;
 + si une question vise un élément académique incompris, nous adresserons celui-ci en classe;
 + aucune demande de solution ne sera tolérée;
 + aucun manque de respect ne sera toléré.

### Vous devez avoir votre propre projet dans votre gestionnaire de version préféré :
+ le fuseau horaire doit être correctement configuré (Montréal);
+ le nom du projet doit être en minuscule et sans faute;
+ les utilisateurs de GitLab doivent s'assurer que la sécurité soit adéquate;
+ vous n'avez pas à créer de répertoire pour vos sources dans ce travail.

# Remise

> >  La totalité de votre travail :
> >  doit être remis le **9 mars 2019** à **23h59** (avec possibilité de bonus)
> >  ou
> >  doit être remis au plus tard le **16 mars 2019** à **23h59**. 
> >  Après cette date, une pénalité de **3 points par jour** de retard sera appliquée.

  La remise se fait **obligatoirement** par l'intermédiaire de l'un des gestionnaires de versions suivants :
  + `GitHub https://github.com/____`;
  + `GitLab https://gitlab.com/____`.
  
> >  Votre projet doit être privé.
  
  **Aucune remise par courriel ne sera acceptée** (le travail sera considéré comme non remis).

  Le nom de votre projet doit être `inf3135-h2019-tp2` (en minuscules). Vous devez donner un accès en
  mode **lecture/écriture** (pas **admin**) à l'utilisateur `guyfrancoeur` (moi-même). Ceci me permettra
  de déposer directement dans vos projets votre note pour le travail ainsi que mes commentaires.
  
  La branche `master` sera celle `clonée` et sera celle qui sera évaluée.

  Votre projet devrait minimalement contenir les fichiers suivants :

- Un fichier `cp.txt` contenant votre code permanent en majuscule et complet (requis pour la publication des résultats);
- Un fichier `tp2.c` contenant le code source de votre projet, ainsi que votre fonction `main`;
- Les fichiers `outils.h` et `outils.c` contenant le code source de vos fonctions;
- Un fichier `README.md` avec le titre du projet, votre approche (réflexion), vos inspirations, les auteurs (bibliographie), etc.;
- Un fichier nommé `Makefile`;
- Un fichier `.gitignore`;
- Un fichier `evaluer.sh`.

# Barème de correction

| Critère | Sous-critère | Points |
| ------- |:------------ | ------:|
| Script (test)     | Script bash pour test `evaluer.sh`               |  2.0 |
| Compilation       | sans avertissement ni erreur                     |  1.0 |
| Fonctionnabilité  | 5 à 10 tests seront lancés (comparaison binaire) |  5.0 |
| Qualité           | temps d'exécution (performance) et code          |  3.0 |
| Makefile          | complet, simple, sans extra                      |  1.0 |
| Contribution      | wiki et issues                                   |  1.0 |
| Réflexion         | Qualité des questions, réponses                  |  1.0 |
| Français          | Français, compréhension                          |  1.0 |
| Bonus             | remise avant le 9 mars 2019 23h59                |  1.0 |
| **Total**         |                                                  | 16/15 |

> > Le bonus ne peut pas être appliqué sur un autre travail.

# TP3

> > Le TP3 sera remis le dans la semaine du 10 mars 2019
