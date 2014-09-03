---
layout: post
title:  "Flat design for Android"
date:   2013-11-12 16:26:26
categories: jekyll update
---


Si vous êtes un utilisateur d’Android, vous devez probablement connaître l’excellente/indispensable application Android File Transfer. Cette petite app vous permet de gérer les fichiers qui sont sur votre device comme vous le feriez avec une clé USB.

Mais tout n’est pas rose au pays des Bisounours. Cette application a la sale petite manie de se lancer automatiquement à chaque fois que vous branchez votre device. Si comme moi, il vous arrive de brancher votre device juste pour développer ou encore pour le recharger, vous n’avez probablement pas envie de voir cette app se lancer automatiquement à chaque fois.
Voici donc la démarche à effectuer pour désactiver tout ça :

<br />

  1. Fermez l’application
  2. Lancez Activity Monitor et killez le process correspondant à Android File Transfer
  3. Rendez vous dans le dossier où est installé Android File Transfer.app (/Applications généralement)
  4. Clic droit sur le package et Show package contents
  5. Allez dans le dossier Contents/Resources
  6. Renommez Android File Transfer Agent en Android File Transfer Agent_STOPIT
  7. Allez dans /Users/username/Library/Application Support/Google/Android File Transfer et renommez à nouveau l’agent

<br />

Et voilà ! L’application ne se lancera plus automatiquement à chaque branchement du device mais restera accessible comme une application classique.
