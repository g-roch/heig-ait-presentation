
Bacula est un set de programmes qui permet à un administrateur réseau de gérer des sauvegarde, la récupération et la vérification de données informatiques sur un réseau d'ordinateurs de différents types. 

Il peut fonctionne sur un seul ordinateur et peut effectuer des sauvegardes sur différents types de supports comme des bandes et des disques.

Bacula est un programme de sauvegarde client/serveur réseau. Il est "facile" d'utilisation et efficace en offrant de nombreuses fonctionnalités avancées de gestion du stockage pour faciliter la recherche et la récupération de fichiers perdus ou endommagés. 

Il est évolutif et peut être utiliser pour de ptits systèmes informatiques simples à des systèmes composés de centaines d'ordinateurs situés sur un grand réseau.

-------------

Si vous utilisez actuellement un programme tel que tar, dump ou bru pour sauvegarder les données de votre ordinateur et que vous souhaitez une solution réseau, plus de flexibilité ou des services de catalogue, Bacula fournira très probablement les fonctionnalités supplémentaires que vous souhaitez. 

Cependant, si vous êtes nouveau sur les systèmes Unix ou si vous n'avez pas d'expérience avec un package de sauvegarde sophistiqué, le projet Bacula ne recommande pas d'utiliser Bacula car il est beaucoup plus difficile à installer et à utiliser que tar ou dump.

Si l'on recherche un programme simple permettant d'écrire sur des bandes, il se peut qu'il soit difficile de travailer avec Bacula.

-> Concu pour protéger les données en suivant des règles spécifiques (choisir par l'administrateur) ce qui indique qu'une bande est réutiliser qu'en cas de secours.
=> si on veut écraser peu importe la bande du lecteur, il est plus facile/efficace d'utiliser un autre programme.

Bacula permet d'écrire sur plusieurs volumes (aucune limite de capacité de la bande). Il serait un programme potentiellement plus simple à installer que d'autres équivalents.

Selon ce qu'on utilise comme  Legato Networker. ARCserveIT, Arkeia ou PerfectBackup+, il peut être intéressant d'utiliser Bacula qui offre un cerrtains nombres de mêmes fonctionnalités et est un logiciel gratuit sous la licence logicielle GNU version 2.

-------------------
Bacula est constitués de 5 composants/services majeurs :
- Director
	permet la supervisions des opérations de sauvegarde, restauration, verification et archivage. L'admin peut l'utiliser pour planifier les sauvegardes et récupérer les fichiers. Il est le composant principal et communique les autres composants.
- Console
	interface permettant à un utilisateur de communiquer avec le composant Director. Il y a trois version. La première est une interface console (shell), une interface graphique QT (GNOME mais pas complète)  et une interface graphique wxWidgets (+ restauration de fichier interactive). 
- client / File 
	logiciel installé sur la machine à sauvegarder. Il est spécifique au système d'exploitation sur lequel il est exécuté et est chargé de fournir les attributs et les données du fichier à la demande du director. Le service est également responsable de la partie de restauration des attributs et des données du fichiers lors des opérations de récupération. Il s'exécute en tant que daemon sur la machine. (Unix/linux + Windows (certains))
- storage
	services qui effectuent le stockage et la restaurations des fichiers et des données sur les supports ou volumes physiques. Les daemon de stockage est responsable de la lecture/écritures des bandes (ou autres supportes). 
- catalog
	composant qui ...
