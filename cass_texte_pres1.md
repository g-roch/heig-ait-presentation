# Texte pour la présentation d'AIT 

## Avantages / Inconvénients

| Avantages                                       | Inconvénients                                            |
| ----------------------------------------------- | -------------------------------------------------------- |
| Interface utilisateur graphique                 | Prise en main complexe (fichiers de configuration)       |
| Cross-platform                                  | Pas de scan de virus                                     |
| Automatisation & planification des tâches       | Configuration nécessaire au backup des appareils mobiles |
| Sauvegarde continue (CDP)                       |                                                          |
| Toujours maintenu (dernière update : juin 2021) |                                                          |
| Sauvegarde Cloud & hors-site                    |                                                          |
| Charge réseau et CPU modulables                 |                                                          |
| Déduplication des données                       |                                                          |
| Support d'environnements virtuels               |                                                          |
| Large documentation & en plusieurs langues      |                                                          |

La courbe d'apprentissage est assez raide, car il faut d'abord prendre en main les **fichiers de configuration** qui ne sont pas bien structurés. Cela prend donc du temps au début, mais permet d'économiser du temps et de l'argent quand on arrive au bout de cette courbe d'apprentissage. 

Par contre, Bacula dispose d'une **interface graphique** qui facilite les choses pour l'utilisateur. 

**Aucun scan de virus** n'est proposé par Bacula, donc si le système est infecté, le virus sera sauvegardé avec le reste des fichiers.

Bacula n'est **pas prévu pour effectuer des sauvegardes d'appareils connectés sporadiquement** mais pour des serveurs avec des adresses IP fixes. Le problème intervient quand l'appareil n'est pas connecté sur le réseau mais que le Director Daemon le cherche malgré tout. Il est tout de même possible de configurer Bacula pour cette situation spécifique avec un script, mais cela ajoute un peu de complexité. 

La solution Bacula est **cross-platform**, elle peut s'installer sur différentes distributions de Linux mais également de nombreuses versions de Windows ainsi que MacOS. On peut installer les différents composants sur FreeBSD, Solaris et OpenSolaris en plus. 

Un autre avantage très recherché est la possibilité d**'automatiser les sauvegardes et de les planifier**. Ainsi pas besoin d'être systématiquement présent pour lancer manuellement les back-ups au moment voulu. 

La **sauvegarde continue** permet de sauver automatiquement tous les changements effectués sur les données d'un client, dès que l'utilisateur les enregistre. 

Bacula est **toujours maintenu**, la dernière update date de juin 2021, ce qui est plutôt récent et indique qu'en cas de souci, un patch sera rapidement disponible. 

Bacula offre une possibilité de **sauvegarde dans le cloud et hors site**. Ces deux possibilités permettent de protéger les données sauvegardées en cas de catastrophe naturelle survenant dans les locaux de l'entreprise. 

Il est possible de **modifier la priorité des processus de sauvegarde pour soulager le CPU,** ainsi que de moduler les types de backup et leur fréquence pour ne pas trop empiéter sur le réseau. 

La **déduplication élimine les copies excessives** de données et réduit considérablement les besoins en capacité de stockage. Elle s'effectue en arrière plan et ne ralentit donc pas la sauvegarde. Bacula utilise également un mécanisme de compression pour réduire la taille des fichiers et accélérer les processus. Cette déduplication des données permet d'alléger la charge réseau engendrée. 

Bacula supporte les **sauvegardes d'environnements virtuels** tels que VMWare, MS Hyper-V, Proxmox ...

La **documentation** disponible est très complète et se trouve en plusieurs langues. 

## Discussion stratégique

Bacula est très flexible et les sauvegardes peuvent être planifiées au bon vouloir de l'administrateur, cela signifie que des backups peuvent être effectués jusqu'à une fois par heure. Cela nous donne un RPO (Recovery Point Objective) très faible. Ce RPO dépend de la manière dont Bacula est configuré. 

Le RPO très faible et l'automatisation possible des sauvegardes engendrent une réelle économie pour l'entreprise, on économise le temps des employés et leur travail qu'on ne risque pas de trop perdre.

