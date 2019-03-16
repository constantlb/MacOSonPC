# MacOSonPC
How to install correctly MacOS on a PC

## Getting Started

Installer le système propriétaire MacOS sur son PC est risqué. Je ne serais responsable si a la suite de la réalisations de ces étapes votre ordinateur ne fonctionne plus!

### Prérequis

Connaitre les informations de son PC :
CPU, GPU, Puce Wifi, Bluetooth, carte son, etc...
Voici un siteweb sympa qui référencie toutes les informations sur les dirérentes puces :
[Wiki Chip](https://en.wikichip.org/wiki/intel/cpuid)

Vous pouvez utiliser la commande `systeminfo` pour faitre apparaitre sur votre terminal les informations de votre système.

Sur Windows vous pouvez aussi ouvrir le menu démarer, et taper Informations Système puis présser entrer. Une fenêtre détaillant l'enssemble de vos composants vas s'ouvrir. Vous pourez prendres notes des choses importantes comme le processeur ou votre carte graphique.

Ce tutoriel vas vous permettre d'installer MacOS Mojave.
Fonctionne uniquement avec les processeurs INTEL.

### Configuration

#### Configurer votre BIOS pour que l'installation de MacOS se déroule correctement.

Redémarer votre PC et appuyer sur la touche qui permet d'accéder au BIOS (F1 ou F2 ou F10 ou F12).

Désactiver l'option de sécurité : `SECURE BOOT`.
Désactiver le démarrage rapide : `FAST BOOT`.

### Installation

Télécharger l'image du système avec le lien suivant: 
[Télécharger MACOS10.14.3](https://drive.google.com/file/d/1malP3BGbC6coziRouv4mnqmJBcY1jFVY/view?usp=sharing)

Télécharger un logiciel qui vous permetra de décomprésser et d'écrire l'image sur un disque, je vous conseile le logiciel open source Etcher disponnible sur Linux et Windows: 
[Télécharger Etcher](https://www.balena.io/etcher)

Graver l'image de MacOS grâce à Etcher sur une clé USB d'une capacité minimun de 8Gb.

Télécharger les pilotes de base pour votre cpu intel : 
