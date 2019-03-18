# MacOSonPC
How to install correctly MacOS on a PC

## A propos

Installer le système propriétaire MacOS sur son PC est risqué. Je ne serais responsable si à la suite de la réalisation de ces étapes votre ordinateur ne fonctionne plus!

Ce tutoriel détaille toutes les étapes pour installer MacOS Mojave.  
Fonctionne uniquement avec les processeurs INTEL.  
Tutoriel testé sur un ThinkPad t470s i7-7500U.

### Prérequis

2 clés USB. 8Gb minimums.

Connaitre les informations de son PC :CPU, GPU, puce Wifi, puce Bluetooth, carte son, etc...  
Surtout le nom et la génération de son CPU, par exemple le mien est le : `i7-7500U` , le chiffre qui suit le `-` correspond à la génération. J'ai donc un CPU INTEL I7 de 7e génération aussi appelée Kaby Lake.
Voici un site web sympa qui référence toutes les informations sur les différents CPU:
[Wiki Chip](https://en.wikichip.org/wiki/intel/cpuid)

Vous pouvez utiliser la commande `systeminfo` pour faitre apparaitre sur votre terminal les informations de votre système.

Sur Windows vous pouvez aussi ouvrir le menu démarrer, et taper Informations Système puis presser entrer. Une fenêtre détaillant l'ensemble de vos composants vas s'ouvrir. Vous pourrez prendres note des choses importantes comme le processeur ou votre carte graphique.

### Configuration

#### Configurer votre BIOS pour que l'installation de MacOS se déroule correctement.

Redémarrer votre PC et appuyer sur la touche qui permet d'accéder au BIOS (F1 ou F2 ou F10 ou F12).

Désactiver l'option de sécurité: `SECURE BOOT`  
Désactiver le démarrage rapide: `FAST BOOT`  
Désactiver la virtualisation: Tout les paramètres  
  
Activer le démarrage UEFI sur USB: `USB UEFI SUPPORT`  
Activer les deux modes de démarrage si disponnible sur votre BIOS: efi et classique: `BOTH (UEFI & LEGACY)`  
Activer la liste des éléments bootables via F12: `BOOT DEVICE LIST`  
  
> En Anglais désactivé se dit: `Disabled` et Activer se dit `Enabled`  

### Installation

Télécharger l'image du système avec le lien suivant: 
[Télécharger MACOS10.14.3](https://epitechfr-my.sharepoint.com/:u:/r/personal/constant_loubier_epitech_eu/Documents/MacOs%20Mojave%2010.14.3/MacOS%20Mojave%2010.14.3.raw.zip?csf=1&e=5lHehQ)

Télécharger un logiciel qui vous permetra de décomprésser et d'écrire l'image sur un disque, je vous conseile le logiciel open source Etcher disponnible sur Linux et Windows: 
[Télécharger Etcher](https://www.balena.io/etcher)

Graver l'image de MacOS grâce à Etcher sur une clé USB d'une capacité minimun de 8Gb.

#### Télécharger les fichiers Clover(Genre de GRUB modifié compatible avec les MacOS maison):

>Télécharger seulement les fichiers correcondant à votre CPU

* Clover pour CPU Intel générations 1 à 5 : Télécharger ces fichiers si votre processeur est d'une fammille:
    * 1ere gen: Nehalem (CPU Intel 2008)
    * 2e gen: Sandy Bridge (CPU Intel 2011)
    * 3e gen: Ivy Bridge (CPU Intel 2012)
    * 4 gen: Haswell (CPU Intel 2013)
    * 5 gen: Broadwell (CPU Intel 2015)  
[Télécharger ici](https://epitechfr-my.sharepoint.com/:u:/r/personal/constant_loubier_epitech_eu/Documents/MacOs%20Mojave%2010.14.3/Clover%201%20a%205%20gen.zip?csf=1&e=YhO34i)

* Clover pour CPU Intel gen 6 et ultérieur installé sur un PC de bureau:
[Télécharger ici](https://epitechfr-my.sharepoint.com/:u:/r/personal/constant_loubier_epitech_eu/Documents/MacOs%20Mojave%2010.14.3/Clover%206+%20gen.zip?csf=1&e=yNhPmo)

* Clover pour CPU Intel gen 6 et ultérieur installé sur un PC portable:
[Télécharger ici](https://epitechfr-my.sharepoint.com/:u:/r/personal/constant_loubier_epitech_eu/Documents/MacOs%20Mojave%2010.14.3/Clover%206+%20gen%20for%20notebooks.zip?csf=1&e=vvvgk4)

#### Imprimer votre première clé USB de l'image systeme MacOS

Ouvrer Etcher: 
* Choisisser l'image macos
* Choisisser votre clé usb
* Appuyer sur Flash!

#### Déplacer les fichiers CLOVER dans la seconde clé USB

Prenez votre dossier qui correspond à votre CPU et déplacer le dans votre deuxième clé.

#### Redémarer

Démarrer votre PC sur la clé qui contient l'image MacOS en utilisant la touche `F12` pour afficher le menu des éléments bootables.  
Choissiser `INSTALL MAC OS MOJAVE`
Si vous êtes sur PC portables, appuyer sur la toucher `o` -> `configs` -> `setup 2`. `echap` x2, puis `entrer`.  
Une fois arriver sur l'interface graphique de l'installation du système :
Séléctionner `Dick Utility` pour choisir ou installer MacOS.  
Puis séléctioner votre disque ou vous souhaitez l'installer.  
A la fin de l'installation, votre PC vas redémarer, refaite `F12`, sélectionner une nouvelle fois votre clé USB. Mais cette fois ci déplacer vous vers le mac os suivis par le nom de votre disque. N'oublier pas : configs -> setup 2 (pour les ordis portables).  
Terminer l'installation.

#### Déplacer les fichiers Clover

Une fois sur MacOS.  
Branchez votre seconde clé usb.  
Déplacer les éléments vers le bureau.  
Vous trouverez à l'intérieur du dossier CLOVER, un fichier d'installation pour ce dernier. Exécuter le.   
Déplacer les fhichiers Clover dans votre système MacOS vers le dossier EFI, en remplacant le dossier existant.  

Félicitations vous avez maintenant créer un HackInToch!  
