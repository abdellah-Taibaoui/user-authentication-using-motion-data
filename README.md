# user-authentication-using-motion-data

*Abstract*—L’authentification biométrique est une méthode d’authentification de l’identité
d’un utilisateur en utilisant des caractéristiques physiques ou comportementales
uniques, telles que les empreintes digitales, la reconnaissance faciale, la reconnaissance de la voix,
la reconnaissance de l’iris ou encore la reconnaissance de
la signature. Contrairement aux mots de passe et aux codes PIN, qui peuvent
être volés, perdus ou oubliés, les caractéristiques biométriques sont propres à
chaque individu et ne peuvent pas être facilement copiées ou falsifiées.

1.  **Methodology**

La reconnaissance de la démarche est une technique basée sur l’analyse des
rythmes associés aux pas effectués lors des mouvements. L’observation du fait
que chaque individu a un style différent de démarche, conduit au développement
de systèmes d’authentification biométriques avancés qui exploitent de telles caractéristiques comportementales. En générale, les techniques de reconnaissance
de démarche sont de trois approches : vision machine, capteur de sol et capteur
portable (Gafurov, 2007). La première approche se base sur les images dans une
vidéo. Les informations de reconnaissances sont déduites à travers l’application
des techniques de traitement d’image et de vidéo.
La seconde approche utilise des capteurs, posés à même le sol, pour recueillir
les informations de la personne qui marche. Cette approche est propice pour le
contrôle d’accès d’un bureau par exemple. La porte s’ouvre à l’identification de
la personne qui marche.
Dans la dernière approche, le capteur qui fait l’enregistrement des données de
la démarche est portée par l’utilisateur.
fait partie de cette dernière approche. Les informations recueillies, pour le traitement, ont souvent besoin de matériels spécialisés. Mais avec l’intégration de
l’accéléromètre dans les smartphones, la reconnaissance de démarche commence
par être exploitée comme méthode d’authentification.
En effet, le smartphone est toujours porté par l’utilisateur dans ses déplacements soit dans la main, soit dans un sac ou dans la poche. Par ailleurs c’est
une méthode qui ne demande aucune action de la part de l’utilisateur donc plus
confortable dans l’utilisation
Comme toute méthode biométrique, la reconnaissance de la démarche commence par l’acquisition des données. Les débuts de cette technologie nécessitaient des appareils spécialisés pour l’acquisition des données. L’évolution technologique a permis l’intégration de plusieurs capteurs tels que les accéléromètres
dans les smartphones. C’est à la suite de cette intégration que l’approche sur la
reconnaissance de la démarche s’est développée sur les smartphone pour devenir
l’une des méthodes biométriques d’authentification sur mobile. Dans l’industrie,
depuis la version 5 Android a intégré le concept de smart Lock. C’est une technologie qui utilise l’environnement du smartphone pour effectuer le verrouillage.
Dans les fonctionnalités, se trouve la reconnaissance de la démarche. En effet,
le smartphone détecte quand son porteur est en mouvement et s’il est déjà déverrouillé, il reste ainsi. Il se verrouille automatiquement quand il est posé ou
il ne détecte plus d’activité. Par contre, il n’identifie pas le porteur.
nous visons à différencier les utilisateurs de téléphones portables en utilisant le
mouvement de la main, l’orientation et la saisie, qui sont collectées à partir de
trois capteurs : accéléromètre (mesure l’accélération moins Gx), gyroscope (mesure l’angle vitesse) et magnétomètre (mesure le champ magnétique ambiant).
Pour chaque capteur, les valeurs des coordonnées X, Y et Z et moment où ces
valeurs sont stockées

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
— Normalisation des données et les Mettre à l’échelle ou normalisez-les pour
éliminer les biais ou les différences d’amplitude entre les différentes séries
temporelles
— Divisez les données en fenêtres de taille fixe avec un overlaping pour faciliter
le traitement et l’analyse ultérieurs.
— Étiquetage des données et Associer chaque segment de données à un utilisateur
— Divisez les données préparées en ensembles d’entraînement, de validation
et de test. L’ensemble d’entraînement est utilisé pour entraîner le modèle,
l’ensemble de validation est utilisé pour ajuster les hyperparamètres et
l’ensemble de test est utilisé pour évaluer les performances du modèle.
