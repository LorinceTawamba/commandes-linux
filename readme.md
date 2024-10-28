# Linux - Les commandes usuelles 

>[!NOTE]
>
>- En général, la plus part des serveurs web ainsi que des serveurs d'application tournent sur Linux. Il est donc bien important pour tout dévéloppeur d'avoir en main les commandes usuelles pour une prise en main rapide. 
>- Voici donc quelques commandes usuelles sous Linux.

## Table de matières 

- [Commande PWD](#Commande-PWD) 
- [Commande CAT](#Commande-CAT) 
- [Commande CLEAR](#Commande-CLEAR)
- [Commande LS](#Commande-LS)
- [Commande CD](#Commande-CD)
- [Commande MKDIR](#Commande-MKDIR)
- [Commande TOUCH](#Commande-TOUCH)
- [Commande CP](#Commande-CP)
- [Commande HELP](#Commande-HELP)
- [Commande MV](#Commande-MV)
- [Commande RM](#Commande-RM) 
- [Commande FIND](#Commande-FIND)
- [Commande GREP](#Commande-GREP)
- [Echainement des commandes](#Echainement-des-commandes)
- [Commande HEAD](#Commande-HEAD)
- [Commande WC](#Commande-WC)
- [Authors](#Authors)
- [License](#License) 

## Commande ***PWD*** 
La commande **PWD** permet de déterminer ou est ce qu'on se trouve dans son arborescence de repertoire.  

>[!NOTE]
>
>- PWD : **P**rint **W**orking **D**irectory.  

- ***Cette syntaxe affiche le résultat de la commande sur la sortie standard.***

```shell
pwd 
```

- ***Cette syntaxe redirige le résultat de la commande vers le début d'un fichier et si le fichier existe déjà, il sera préalablement vidé de son contenu.***

```shell
pwd > nom-du-fichier.txt
```

- ***Cette syntaxe redirige le résultat de la commande vers la fin d'un fichier***

```shell
pwd >> nom-du-fichier.txt
```

## Commande ***CAT*** 
La commande **CAT** permet d'afficher le contenu d'un fichier.   

>[!NOTE]
>
>- CAT : Concatenate.  

- ***Cette syntaxe affiche le contenu du fichier sur la sortie standard.***

```shell
cat nom-du-fichier.txt
```

## Commande ***CLEAR*** 
La commande **CLEAR** permet d'effacer l'écran.   

- ***Cette syntaxe efface l'écran.***

```shell
clear
```

## Commande ***LS*** 
La commande **LS** permet de lister tous les repertoire se trouvant dans le repertoire ou je me situe actuellement.  

>[!NOTE]
>
>- PWD : **P**rint **W**orking **D**irectory.  

- ***Cette syntaxe affiche la liste des repertoires et fichiers sur la sortie standard.***

```shell
ls 
```

- ***Cette syntaxe affiche la liste des repertoires et fichiers avec leurs propriété sur la sortie standard.***

```shell
ls -al
```

## Commande ***CD*** 
La commande **CD** permet de lister tous les repertoire se trouvant dans le repertoire ou je me situe actuellement.  

>[!NOTE]
>
>- CD : **C**hange **D**irectory.  

- ***Cette syntaxe permet de se déplacer d'un repertoire à un autre.***

```shell
cd nom-du-repertoire 
```

- ***Cette syntaxe permet de revenir sur ses pas un cran en arrière.***

```shell
cd .. 
```

## Commande ***MKDIR*** 
La commande **MKDIR** permet de lister tous les repertoire se trouvant dans le repertoire ou je me situe actuellement.  

>[!NOTE]
>
>- MKDIR : **M**ake **D**irectory.  

- ***Cette syntaxe permet de créer un nouveau repertoire.***

```shell
mkdir nom-du-repertoire 
```

- ***Cette syntaxe permet de créer un nouveau sous repertoire dans repertoire.***

```shell
mkdir -p nom-du-repertoire/nom-du-sous-repertoire 
```

>[!TIP]
>
> -p : Cette option permet de créer le repertoir parent s'il n'existe pas. 

## Commande ***TOUCH*** 
La commande **TOUCH** permet de créer un nouveau fichier.

- ***Cette syntaxe permet de créer un nouveau fichier.***

```shell
touch nom-du-fichier.txt 
```

- ***Cette syntaxe permet de créer un nouveau fichier dans un repertoire spécifique.***

```shell
touch nom-du-repertoire/nom-du-fichier.txt 
```

## Commande ***ECHO*** 
La commande **ECHO** permet d'écrire un contenu sur la sortie standard ou dans un fichier. 

- ***Cette syntaxe permet d'écrire un contenu sur la sortie standard.***

```shell
echo "Votre contenu" 
```

- ***Cette syntaxe permet d'écrire un contenu dans un fichier existant.***

```shell
echo "Votre contenu" > nom-du-fichier.txt 
```

## Commande ***CP*** 
La commande **CP** permet de copier un fichier d'une source à un autre. 

>[!NOTE]
>
>- CP : **C**opy. 

- ***Cette syntaxe permet d'écrire un contenu sur la sortie standard.***

```shell
cp nom-du-fichier.txt destination/ 
``` 

## Commande ***HELP*** 
La commande **HELP** permet d'avoir la documentation sur la commande. 

- ***Cette syntaxe permet d'avoir la documentation sur la commande MKDIR.***

```shell
mkdir --help 
```

## Commande ***MV*** 
La commande **MV** permet de déplacer ou renomer un fichier. 

>[!NOTE]
>
>- MV : **M**ove. 

- ***Cette syntaxe permet de déplacer ou renomer un fichier.***

```shell
mv nom-du-fichier-source.txt  nom-du-fichier-destination.txt 
```

## Commande ***RM*** 
La commande **RM** permet de supprimer un fichier. 

- ***Cette syntaxe permet de déplacer ou renomer un fichier.***

```shell
rm nom-du-fichier.txt 
```

## Commande ***FIND*** 
La commande **FIND** permet de rechercher un fichier. 

- ***Cette syntaxe permet de faire la recherche a partir d'une source.***

```shell
find source-de-la-recherche -name "element-de-la-recherche"  
```

## Commande ***GREP*** 
La commande **GREP** permet de faire la recherche d'une chaine dans un fichier. 

- ***Cette syntaxe permet de faire la recherche d'une chaine dans un fichier.***

```shell
grep "element-de-la-recherche" cyble-de-la-recherche  
```

- ***Exemple.***

```shell
grep "projet" *.md  
```

## Enchainement des commandes 

>[!TIP]
>
> && : permet d'enchainer les commandes les une a la suite des autres.  

- ***Cette syntaxe permet de faire la recherche d'une chaine dans un fichier.***

```shell
mkdir test && cd test   
```

## Commande ***HEAD*** 
La commande **HEAD** permet de lire une section ou une partie d'un fichier. 

- ***Cette syntaxe permet de lire les 5 premieres lignes de mon fichier.***

```shell
head -n 5 nom-de-mon-fichier.txt
```

## Commande ***WC*** 
La commande **WC** permet de compter le nombre de mots dans un fichier. 

>[!NOTE]
>
>- WC : **W**ord **C**ount. 

- ***Cette syntaxe permet de compter le nombre de mots dans un fichier.***

```shell
wc nom-du-fichier.txt  
```

# Authors

* **Lorince TAWAMBA** _alias_ [@LorinceTawamba](https://github.com/LorinceTawamba)

Read the list of [contributors](https://github.com/lorince-tawamba/gescom/contributors) to see who helped with the project ! 

# License

Ce document est placé sous licence CC BY-NC-SA :  [Creative Commons
Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions](https://creativecommons.org/licenses/by-nc-sa/4.0/)

![Logo](https://licensebuttons.net/l/by-nc-sa/3.0/88x31.png)

En savoir plus sur [les licences Creative Commons](https://creativecommons.org/licenses/?lang=fr-FR)...
