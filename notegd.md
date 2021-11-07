## Présentation 

#### Introduction

Bacula est un logiciel de sauvegarde multi-platforme. Il a été développé à partir de l'année 2000 par Kern Sibbald et sa première version a été publiée deux ans plus tard, c'est-à-dire en 2002. 

Le logiciel est continuellement maintenu, documenté et mis à jour. Pour vous donnez une idée, la dernière release est sortie en juin de cette année. 

Bacula possède une version community qui est Open Source. Ses différents composants peuvent tourner sur des systèmes d'exploitation gratuit (par ex linux) ce qui ne nécessite pas l'achat de licences supplémentaires pour tester le logiciel.

Il existe une version entreprise avec plus de fonctionnalités mais cette fois-ci payante que l'on vous présentera par la suite.

#### Architecture

Bacula est composé de 5 composants principaux :

- **Director** : il suppervise les opérations de sauvegarde, restauration, verification et archivage. C'est le composant principal et le point central des intéractions entre les composants.
- **Console** : c'est l'interface qui permet aux utilisateurs de communiquer avec le composant Director. Il existe 2 versions :  un shell et une interface web.
- **Client (file daemon)** : logiciel installé sur les machines clientes. Il est spécifique à l'OS sur lequel il est présent. Il sera chargé de transmettre les données à sauvegarder et est utilisés pour les opérations de récupérations.  
- **Storage** : composant responsable de l'écriture des sauvegardes sur les médias choisi: Par exemple sur des disques, les bandes et dans le cloud.
- **Catalog** : est responsable de la maintenance des index de fichiers pour tous les fichiers sauvegardés et stock les info sur les différentes sauvegardes réalisées.

#### Chiffrement

En ce qui concerne le chiffrement, Bacula permet de chiffrer et signer les données qui sont a backup dans le storage. Les données sont chiffrées autant dans la transmission que dans le backup.

- Il faut tenir compte que seul le contenu des fichiers est chiffrés/signé alors que les métadonnées ne le sont pas (ça concerne par exemple : le nom du fichier, les permissions et le propriétaire du fichier).
- Attention, il est important d'avoir plusieurs sauvegardes de la master key utilisé pour le chiffrement car si on la perd, toutes les données chiffrées seront perdu.
- Communication via TLS => chiffrée

