# projet_econometrie
Ce dossier contient toutes les données que nous avons récolté depuis le début de notre projet. 

Le dossier "Data" contient les données que nous avons utilisé pour notre projet.
Le sous dossier "donnees_brutes" qui contient les fichiers excel que nous avons téléchargé soit du site de la banque mondiale, soit du site Our World In Data (abrégé en OWID). 
L'excel "data_agregee" est un .xlsm qui contient les données retraitées que nous utilisons dans GRETL et desquelles nous tirons nos résultats. Ce fichier contient aussi la macro VBA permet retraité les données. Comme mentionné dans le pdf certaines valeurs sont manquantes pour des pays particuliers et il a donc été nécessaire d'exclure des pays pour lesquels toutes nos variablse n'étaient pas observées. 
Cependant, la macro ne contient pas tous les retraitement. En effet nous avons enlevé, "à la main" les régions crée par la banque mondiale et ou par convention. 

Le sous-dossier "donnees_retraitees" contient les données qui on été nettoyées "à la main" et pour lesquelles nous avons créé la variable "GINI_binaire".
- Le fichier "data_agregee_main.xlsm" nous permet de créer la variable binaire grace à la formule "=SI($G4<=$J$3;0;1)" dans la colonne H. De plus nous calculons la médiane dans la case J3. 
- Le fichier "data_agregee_CSV.utf-8" est le fichier final qui sera utilisé par Gretl et qui est nettoyé de toutes les données inutiles. 

Le dossier "projet_latex" contient les fichiers que nous avons utilisé afin de générer le rapport qui est écrit en latex. Nous avons utilisé l'extension VSCode Latex Workshop à cette fin. 

Le dossier "GRETL" contint quant à lui le fichier gretl sur lequel nous avons effectué nos calculs et aussi où sont enregistré les graphiques et tableaux qu'on utilise dans le fichier .tex dans le dossier précédent. 

Enfin le dossier contient un pdf qui est la version compilée de notre projet qui a été compilé.

SOURCES & LIENS : 
	- Espérance de vie à la naissance : https://donnees.banquemondiale.org/indicateur/SP.DYN.LE00.IN
	- PIB/hab en PPA : https://donnees.banquemondiale.org/indicateur/NY.GDP.PCAP.PP.CD
	- taux de scolarisation dans le secondaire : https://data.worldbank.org/indicator/SE.SEC.ENRR 
	- Indice de GINI : 
https://ourworldindata.org/grapher/gini-coefficient-wid-vs-pip
