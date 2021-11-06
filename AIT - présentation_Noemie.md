# AIT - présentation

> 25.10.2021

## Coûts

Il existe deux versions de Bacula, une version community qui est open-source, donc gratuite et une version entreprise qui est payante sous forme d'abonnement mensuel.

> Bacula Enterprise Edition est la solution phare de sauvegarde et  restauration distribuée, en réseau, Open Core, prête pour les  déploiements en production. L'édition "Enterprise" de Bacula fourni des  fonctions avancées, autonomes et certifiées, utilisables directement en  production vous économisant des ressources internes de R&D. En  dédiant directement à un expert le traitement des demandes, Bacula  Systems apporte un support technique de très haute qualité dans les  délais qui garantissent ses engagements contractuels. La version  Communautaire de Bacula est adaptée à une utilisation d'évaluation ou de pré-production. Pour son utilisation en environnement de production en  entreprise, la version Communautaire requiert des ressources internes  pour en gérer les mises à jour, la tester, prendre en charge son support et y ajouter des fonctionnalités avancées à celles de base disponibles.

Il est possible de télécharger une version d'essai afin de voir toutes les différentes fonctionnalités.

> https://www.baculasystems.com/fr/sauvegarde-open-source-loffre-selective-migration-plan/comparaison-entre-enterprise-edition-et-communautaire/

![image-20211025144050879](/home/noemie/.config/Typora/typora-user-images/image-20211025144050879.png)

Il existe donc 6 abonnements d'assistances différents qui est lié aux nombres de client/serveurs à sauvegarder et le nombre de plateformes différentes (systèmes d'expoitations):

![image-20211025144117664](/home/noemie/.config/Typora/typora-user-images/image-20211025144117664.png)

Au niveau du coût total annuel de chaque abonnement, il est nécessaire de prendre contact avec Bacula afin de nos besoins spécifiques ainsi que notre projet de sauvegarder et restauration. Les bureaux principaux se trouvent à Yverdon.

--> meilleur choix à faire serait la version Bronze (temps d'assistance assez rapide, nombre de client/serveurs assez larges -> possibilité d'ajouter des serveurs à tout moment)

### Dépendances

### Comparaisons

https://en.wikipedia.org/wiki/Comparison_of_backup_software

> https://www.itarian.com/msp-tools/bacula-vs-rsync.php

Rsync

> https://www.toolbox.com/tech/enterprise-software/articles/amanda-vs-bacula-backup-software/

Amanda

backupborg

------

Bacula existe en deux versions différentes, une version community (qui est open-source) et une version entrerprise, qui est donc payante.

La version payante apporte quelques fonctionnalités en plus que la community; entre autres elle met un disposition un expert qui permet d'apporter un support technique ainsi qu'une assitance pour répondre aux questions.

A propos de la version communautaire, elle demande plus de ressources internes afin gérer les mises à jour, la tester, prendre en charge son support et y ajouter des fonctionnalités avancées à celles de base disponibles.

-> donc la version Entreprise est plus appropriée pour les backups d'entreprise et de plus grosse infrastructure à sauvegarder.

Il existe donc plusieurs abonnements différents, 5 différents, qui sont en fonction du niveau d'assistance et du temps de réponse du support.

Il y a plusieurs options différentes dans ces abonnements:

On remarque donc qu'ils dépendent du nombre de clients (machines et serveurs) à sauvegarder. 

Il y a également l'option du temps de réponse du support qui dépendra donc du niveau de sévérité de la panne (il y a 4 niveaux différents, 4 étant la plus sévère). On voit qu'au plus vite un expert peut intervenir dès 1h après une panne de grande sévérité. Je précise que ce sont seulement des jours ainsi que des heures ouvrables, donc le week-end n'est pas inclu.

Au niveau du coût total annuel de chaque abonnement, il est nécessaire de prendre contact avec Bacula afin de définir nos besoins spécifiques ainsi que notre projet de sauvegarde et restauration pour qu'ils fassent un devis. Il est également possible de télécharger une version d'essai de 1 mois afin de tester toutes les fonctionnalités ainsi que le support !! Mais on peut compter au minimum 500$ par mois pour l'abonnement standard.

--> au niveau des abonnements à prendre, tout dépend du besoin de disponibilité des données:

- Entreprise de recherche en informatique par exemple, à ce moment là le temps de réponse du support pourrait être un peu plus large car ils peuvent stopper leur recherche pendant un peu plus de temps et il n'y aura pas de répercussion
- Entreprise qui possède un site web, à ce moment, en cas de panne sévère, si le service est down, il est impératif de dépanner au plus vite afin de rendre le site web à nouveau disponible

Donc comme je l'ai dit avant, il est préférable de prendre contact directement avec Bacula et de demander un devis afin de trouver le meilleur abonnement pour l'entreprise.

Les bureaux principaux se trouvent à Yverdon. Donc il est possible de les contacter par téléphone ou de directement passer dans les bureaux.



Les outils que je vais comparer avec Bacula c'est BorgBackup, Bup, Duplicati ainsi que rsync.

Bacula propose deux versions de son logiciel, une gratuite qui est open source et une autre payante. BorgBackup propose également ces deux options. Sinon tous les outils propose une version gratuite et open-source.

Bacula permet d'effectuer des backups de 3 manières différentes, full/incrémental/différentiel, BorgBackup le permet aussi. Sinon l'outil Duplicati propose le backup différentiel en moins.

La plupart des outils comparés peuvent être utilisés avec les systèmes d'exploitation Linux, MacOS et Windows. Il y a juste BorgBackup et Bup qui ne supporte pas Windows.

-> on constate finalement que Bacula est un outil complet qui est assez flexible. Mais BorgBackup peut également être une alternative possible, mais seulement si on n'utilise pas Windows.

> Comparaison avec Rsync

Logiciel gratuit et open source. Permet de faire des backups incrémentaux mais ne permet pas de faire des manipulations plus complexes et ne chiffre pas les données de backup.  -> outil assez simple plutôt pour des plus petites infrastructure

> Comparaison avec BorgBackup

Logiciel gratuit et open source. Comme pour Bacula, il a aussi un service payant afin d'offrir du support et des solutions de stockages (les prix sont en fonction du service). Possibilité de faire des backups full/incrémentaux/différentiels comme Bacula. Propose la déduplication. Supporte la compression des données ainsi que les données chiffrées.

--> Ne tourne pas sur Windows.

> Comparaison avec Duplicati

Logiciel gratuit et open source. Backups full et incrémentauy. Chiffre les données et supportent les fichiers chiffrés. Deduplication, fonctionne sur Windows, Linux et MacOS.

> Comparaison avec Bup

Logiciel gratuit et open source. Possibilité de faire des backup incrémentaux et de la deduplication. En comparaison à Bacula, Bup ne fait pas du chiffrement de données backup et il n'a pas d'interface graphique directement proposée avec l'outil (il faut télécharger un outil à côté -> Bups).