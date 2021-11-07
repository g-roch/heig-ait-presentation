## Présentation 

#### Introduction

Bacula est un logiciel de sauvegarde multi-platforme. Il a été développé à partir de l'année 2000 par Kern Sibbald et sa première version a été publiée deux ans plus tard, c'est-à-dire en 2002. 

Le logiciel est continuellement maintenu, documenté et mis à jour. Pour vous donnez une idée, la dernière release est sortie en juin de cette année. 

Bacula possède une version community qui est Open Source. Ses différents composants peuvent tourner sur des systèmes d'exploitation gratuit (par ex linux) ce qui ne nécessite pas l'achat de licences supplémentaires à acheter pour tester le logiciel.

Il existe une version entreprise avec plus de fonctionnalités mais cette fois-ci payante que l'on vous présentera par la suite.

#### Architecture

Bacula est composé de 5 composants principaux :

- **Director** : il suppervise les opérations de sauvegarde, restauration, verification et archivage. C'est le composant principal et le point central des intéractions entre les composants.
- **Console** : c'est l'interface qui permet aux utilisateurs de communiquer avec le composant Director. Il existe 2 versions :  un shell et une interface web.
- **Client** : logiciel installé sur les clients qui doivent être sauvegardés. Il est spécifique à l'OS sur lequel il est présent. Il sera chargé de transmettre les données à sauvegarder et utilisés pour les opérations de récupérations. 
- **Storage** : composant responsable de l'écriture des sauvegardes sur les médias choisi. Les médiums de backup supportés sont les disques, les bandes et le cloud ce qui est assez classique pour les sauvegardes. 
- **Catalog** : est responsable de la maintenance des index de fichiers pour tous les fichiers sauvegardés.

#### Chiffrement

En ce qui concerne le chiffrement, Bacula permet de chiffrer et signer les données qui sont a backup dans le storages (transmission entre Storage Daemon et Client). 

- Les données sont chiffrées autant dans la transmission que dans le stockage du backup.

- Attention, seul le contenu des fichiers est chiffrés/signé alors que les métadonnées ne le sont pas (on connait donc le nom, les permissions et le propriétaire du fichier).

