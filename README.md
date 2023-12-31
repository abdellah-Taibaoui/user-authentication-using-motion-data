# user-authentication-using-motion-data

*Abstract*—L’authentification biométrique est une méthode d’authentification de l’identité
d’un utilisateur en utilisant des caractéristiques physiques ou comportementales
uniques, telles que les empreintes digitales, la reconnaissance faciale, la reconnaissance de la voix,
la reconnaissance de l’iris ou encore la reconnaissance de
la signature. Contrairement aux mots de passe et aux codes PIN, qui peuvent
être volés, perdus ou oubliés, les caractéristiques biométriques sont propres à
chaque individu et ne peuvent pas être facilement copiées ou falsifiées.

1.  **Methodology**

La reconnaissance de la démarche repose sur l'analyse des rythmes liés aux pas, utilisant des approches telles que la vision machine, les capteurs de sol et les capteurs portables. Cette dernière approche, intégrant les smartphones avec des capteurs comme l'accéléromètre, émerge comme une méthode biométrique pratique sans nécessiter d'action de l'utilisateur. Dans le contexte des smartphones, la reconnaissance de la démarche est utilisée dans des fonctionnalités telles que Smart Lock sur Android, exploitant le mouvement du smartphone pour le verrouillage. Notre objectif est de différencier les utilisateurs de téléphones portables en utilisant des données de mouvement de la main, de l'orientation et de la saisie provenant d'accéléromètres, gyroscopes et magnétomètres.

2.  **DATASET**

Pour créer le modele d’identifaction d’utilisateur on a travaillié avec H-MOG
Dataset .
cette dataset qui etait publiés en 2015 par l’Institut de Technology du New
York , capture discrètement les subtils micro-mouvements et les dynamiques
d’orientation résultant de la manière dont un utilisateur saisit, tient et tape sur
un smartphone. Les données ont été collectées dans deux conditions : assis et
en marche, et ont été extraites à un taux d’échantillonnage du capteur de 16
Hz.
Cette dataset contient les donnés de mouvment du 100 personnes pour 24 sessions et chaque sessions dure 15 min
Nous avons utilisé un ensemble de données comprenant 4 personnes pour 14
sessions .


3.  **la préparation des données**
   
pour la préparation des données on a passées par plusieurs étapes :

-   Normalisation des données et les Mettre à l’échelle ou normalisez-les pour
éliminer les biais ou les différences d’amplitude entre les différentes séries
temporelles

-   Divisez les données en fenêtres de taille fixe avec un overlaping pour faciliter
le traitement et l’analyse ultérieurs.

-   Étiquetage des données et Associer chaque segment de données à un utilisateur

-   Divisez les données préparées en ensembles d’entraînement, de validation
et de test. L’ensemble d’entraînement est utilisé pour entraîner le modèle,
l’ensemble de validation est utilisé pour ajuster les hyperparamètres et
l’ensemble de test est utilisé pour évaluer les performances du modèle.


