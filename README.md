# ProjetData354
##Présentation

  L'objectif de ce défi est de prédire la maladie d'une plante de riz à partir d'images RGB et infrarouges. 
  
En effet la détection précoce des maladies des cultures, comme la pyriculariose, est cruciale, mais elle est souvent compliquée par la confusion fréquente avec la tache brune. Ces deux maladies fongiques présentent des similitudes visuelles à leurs débuts. Avec le manque d'experts en vulgarisation agricole dans le pays, l'utilisation des avancées récentes en vision par ordinateur, notamment avec des images multispectrales, est nécessaire pour faciliter un diagnostic précoce.
 
#

I- PRISE EN MAIN ET EXPLORATION ET PREPARATION DES DONNEES

Pour la réalisation du projet, nous avons reçu un dossier Image, un fichier Train.csv que nous devons utiliser pour entraîner nos modèles et un fichier Test.csv que  nous devons utiliser pour tester les performances de nos modèles.

Nous avons dans un premier temps effectué une analyse exploratoire sur le fichier Train.csv. On a remarqué qu'il contenait les identifiants des images prises par un téléphone et celles prises par une caméra à infrarouge. Ayant décidé de ne travailler qu'avec un seul type d'image suivant les consignes du challenge, j'ai supprimé les identifiants des images à infrarouge de mon Train.csv. J'ai ensuite exploré, analyser et encodé les modalités de ma variable cible. Ceci est capitale dans tout projet de Data Science qui traite des variables qualitatives.

Notre problème étant un problème de Deep Learning car il est question d'images (données non structurées), j'ai estimé que notre ensemble d'entrainement était trop petit de taille pour l'entraînement de modèles de Deep Learning. J'ai donc créé des blocs de données afin de faire de la validation croisée qui permettre à notre modèle de mieux apprendre des données d'entrainement.  

II- IMPLEMENTATION ET ENTRAINEMENT DE MODELE
 Après essaie de différents modèles, j'ai retenu le modèle ResNet-18 quia été celui qui m'a donné les meilleures performance en aprentissage et en test.
 
 Pour l'implémentation du modèle, j'ai importer les bibliothèque dédiées qui m'on permit dans un premier de faire des prétraîtements sur mes images afin   
qu'elles puissent être mieux adptées à notre modèle.

Pour la mise 




