# int-gration-continue

ThomasB / MaxenceP / AstinL

## Prérequis

- Vagrant : Assurez-vous que Vagrant est installé sur votre machine.
- VirtualBox : Utilisé comme fournisseur de machine virtuelle.
- Accès à Internet : Pour télécharger GitLab et ses dépendances.


## Installation

Danbs le dossier voulu executer :
```
vagrant init
```
Cela créer le vagrant file. Remplacer son contenu avec le notre.

Afin de l'executer nous faisons un : 
```
vagrant up
```

On peut se connecter sur la machine avec un 
```
vagrant ssh
```
Pour se connecter au Git nous ouvrons notre navigateur et allons sur :

localhost:8080

Le Git peut mettre quelques minutes à demarrer.

Les logins par défaut sont root et pour le mot de passe nous faisons :
```
sudo cat /etc/gitlab/initial_root_password
```
Ceci est un mot de passe éphémère, il faudra le changer par la suite.


