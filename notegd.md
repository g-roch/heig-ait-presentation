
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

----------------

## Présentation 

#### Introduction

Bacula est un logiciel de sauvegarde multi-platforme. Il a été développé à partir de l'année 2000 par Kern Sibbald et sa première version a été publiée deux ans plus tard, c'est-à-dire en 2002. 

Le logiciel est continuellement maintenu, documenté et mis à jour régulièrement. Pour vous donnez une idée, nous avons la dernière release (11.0.5) en juin de cette année. 

Bacula est Open Source. Ses différents composants peuvent tourner sur des systèmes d'exploitation gratuit (linux, FreeBSD, Solaris) ce qui ne nécessite pas l'achat de licences supplémentaires à acheter.  Il est donc possible de tester le logiciel gratuitement.

Il existe une version entreprise mais cette fois-ci payante que l'on vous présentera par la suite.

#### Architecture

Bacula est composé de 5 composants principaux :

- Director : il suppervise les opérations de sauvegarde, restauration, verification et archivage. C'est le composant principal et le point central des intéractions entre les composants.
- Console : c'est l'interface qui permet aux utilisateurs de communiquer avec le composant Director. Il existe 2 versions :  un shell et une interface web.
- Client : logiciel installé sur les clients qui doivent être sauvegardés. Il est spécifique à l'OS sur lequel il est présent. Il sera chargé de transmettre les données à sauvegarder et utilisés pour les opérations de récupérations. 
- Storage : est le logiciel qui effectue le stockage des fichiers sur les supports ou volumes physiques. 
- Catalog : est responsable de la maintenance des index de fichiers pour tous les fichiers sauvegardés.

https://www.baculasystems.com/trial-documentation/introducing-bacula-enterprise/



Chiff

https://www.baculasystems.com/wp-content/uploads/2020/Bacula_Enterprise_Edition_for_the_Cloud_s.pdf

https://www.bacula.org/11.0.x-manuals/en/main/Data_Encryption.html

https://www.bacula.org/11.0.x-manuals/en/main/Bacula_TLS_Communications_E.html
