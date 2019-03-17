# MacOSonPC
How to install correctly MacOS on a PC

## A propos

Installer le système propriétaire MacOS sur son PC est risqué. Je ne serais responsable si a la suite de la réalisations de ces étapes votre ordinateur ne fonctionne plus!

Ce tutoriel détailes toutes les étapes pour installer MacOS Mojave.  
Fonctionne uniquement avec les processeurs INTEL.  
Tutotiel tester sur un ThinkPad t470s i7

### Prérequis

Disposais de 2 clés USB. 8Gb minimum.

Connaitre les informations de son PC :
CPU, GPU, Puce Wifi, Bluetooth, carte son, etc...
Voici un siteweb sympa qui référencie toutes les informations sur les dirérentes puces :
[Wiki Chip](https://en.wikichip.org/wiki/intel/cpuid)

Vous pouvez utiliser la commande `systeminfo` pour faitre apparaitre sur votre terminal les informations de votre système.

Sur Windows vous pouvez aussi ouvrir le menu démarer, et taper Informations Système puis présser entrer. Une fenêtre détaillant l'enssemble de vos composants vas s'ouvrir. Vous pourez prendres notes des choses importantes comme le processeur ou votre carte graphique.

### Configuration

#### Configurer votre BIOS pour que l'installation de MacOS se déroule correctement.

Redémarer votre PC et appuyer sur la touche qui permet d'accéder au BIOS (F1 ou F2 ou F10 ou F12).

Désactiver l'option de sécurité : `SECURE BOOT`  
Désactiver le démarrage rapide : `FAST BOOT`

### Installation

Télécharger l'image du système avec le lien suivant: 
[Télécharger MACOS10.14.3](https://epitechfr-my.sharepoint.com/:u:/r/personal/constant_loubier_epitech_eu/Documents/MacOs%20Mojave%2010.14.3/MacOS%20Mojave%2010.14.3.raw.zip?csf=1&e=5lHehQ)

Télécharger un logiciel qui vous permetra de décomprésser et d'écrire l'image sur un disque, je vous conseile le logiciel open source Etcher disponnible sur Linux et Windows: 
[Télécharger Etcher](https://www.balena.io/etcher)

Graver l'image de MacOS grâce à Etcher sur une clé USB d'une capacité minimun de 8Gb.

##### Télécharger les fichiers Clover(Genre de GRUB modifié pour MacOS maison):

>Télécharger seulement les fichiers correcondant à votre CPU

* Clover pour CPU Intel générations 1 à 5 : Télécharger ces fichiers si votre processeur est d'une fammille:
    * 1ere gen: Nehalem (CPU Intel 2008)
    * 2e gen: Sandy Bridge (CPU Intel 2011)
    * 3e gen: Ivy Bridge (CPU Intel 2012)
    * 4 gen: Haswell (CPU Intel 2013)
    * 5 gen: Broadwell (CPU Intel 2015)  
[Télécharger ici](https://epitechfr-my.sharepoint.com/:u:/r/personal/constant_loubier_epitech_eu/Documents/MacOs%20Mojave%2010.14.3/Clover%201%20to%205%20gen.zip?csf=1&e=0G6kRp)

* Clover pour CPU Intel gen 6 et ultérieur installé sur un PC de bureau:
[Télécharger ici](https://epitechfr-my.sharepoint.com/:u:/r/personal/constant_loubier_epitech_eu/Documents/MacOs%20Mojave%2010.14.3/Clover%206+%20gen.zip?csf=1&e=5Y6qy6)

* Clover pour CPU Intel gen 6 et ultérieur installé sur un PC portable:
[Télécharger ici](https://epitechfr-my.sharepoint.com/:u:/r/personal/constant_loubier_epitech_eu/Documents/MacOs%20Mojave%2010.14.3/Clover%206+%20gen%20for%20notebooks.zip?csf=1&e=8tUO2L)


