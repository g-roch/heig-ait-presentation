# AIT - Présentation 1 - Notes

> Cassandre Wojciechowski

## Sujet : Bacula

- Give a presentation of 16 minutes about the chosen subject. It will be followed by 2 minutes of Q&A.
  - Discuss advantages/disadvantages, costs, dependencies. If possible, compare with other solutions. Have a technical discussion, but also a strategic one (take the viewpoint of the CEO).
  - Include a live demo of the software/service.
  - Deliver a PDF of the slides.
- Write a document destined for a system administrator that contains a summary of the most important points to know about the software/service. A kind of cheat sheet with an overview, how to install/configure/use/... Do not simply repeat the slides. Deliver a PDF of the document.

______________________________________

**Is the code Open Source? Is at least the data format open and documented?**

Bacula est open source.

**Does it have cross-platform support?**

Yes : 

![image-20211020150457110](/home/cassandre/.config/Typora/typora-user-images/image-20211020150457110.png)

Src : https://www.bacula.org/what-is-bacula/supported-operating-systems/

**What backup media are supported?**

Tape and disk + ...

**How heavy is a backup in terms of time, CPU load, network load?**



**Can it do fully automated backups without user intervention?**

Oui (?)

**Are mobile devices supported that are connected only sporadically?**



**Is the data encrypted? In transit? At rest?**

TLS -> PSK = pwd set in the daemons

> Src : https://www.bacula.org/automatic-tls-encryption/

**What's the RPO?**



**How easy is it to restore a single file that was accidentally overwritten two weeks ago?**

"[...] offering many advanced storage management features that make it easy to find and recover lost or damaged files."

Normalement, cela doit être très simple car Bacula ne va jamais réécrire sur le même média (c'est le dernier recours).

"[...] the catalog maintains a record of all Volumes used, all Jobs run, and all Files saved, permitting efficient restoration."

> Src : https://www.bacula.org/what-is-bacula/



Director / Console / File / Storage / Monitor