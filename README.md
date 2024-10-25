
# int-gration-continue

ThomasB / MaxenceP / AstinL

## Prérequis

- Vagrant : Assurez-vous que Vagrant est installé sur votre machine.
- VirtualBox : Utilisé comme fournisseur de machine virtuelle.
- Accès à Internet : Pour télécharger GitLab et ses dépendances.


## Installation

Dans le dossier voulu exécuter :
```
vagrant init
```
Cela crée le vagrantFile. Remplacer son contenu avec le nôtre.

Afin de l'exécuter nous faisons un : 
```
vagrant up
```

On peut se connecter sur la machine avec un 
```
vagrant ssh
```
Pour se connecter au Git, nous ouvrons notre navigateur et allons sur :

localhost:8080

Le Git peut mettre quelques minutes à démarrer.

Les logins par défaut sont root et pour le mot de passe nous faisons :
```
sudo cat /etc/gitlab/initial_root_password
```
Ceci est un mot de passe éphémère, il faudra le changer par la suite (utiliser la commande : sudo gitlab-rake "gitlab:password:reset" ).
```
```
# ATELIER 2
** Nous avons fournit au sein du repository, les fichiers yml et dockerfile. **
** Il fallait également fournir un scrpt d'initialisation des runners. N'ayant pas fait de scripts, nous allons décrire étape par étape avec des illustrations ce que nous avons fait. **

## Aller dans Settings -> CI/CD -> Runners
## Cliquer sur "New project Runner"
![image](https://github.com/user-attachments/assets/6ea23761-b88a-4fd9-bdad-5db6f7ddf9ba)

## Ajouter des tags et cliquer la case "Run Untagged jobs"
## Cliquer sur create runner

![image](https://github.com/user-attachments/assets/db647ad7-24cc-4da3-a755-bf12358409be)

## Si "plantage" ajouter le port à l'URL pour afficher les détails du runner et le token
![image](https://github.com/user-attachments/assets/d6cb20d0-8993-4ee4-bef4-400632616e18)

## Après quelques lignes de commandes, nous avons notre runner fonctionnel : 
![image](https://github.com/user-attachments/assets/2157dc87-f5db-4613-bca1-3b597c4caacd)
----
## Pipeline fonctionnelle : 
![image](https://github.com/user-attachments/assets/eca65ebd-0e1e-4ec8-a7b2-b6159fb2decc)

-----------------
# ATELIER 3

## Smoke Test Job : 
![image](https://github.com/user-attachments/assets/e8647997-6e56-4a96-9d77-9527b1577c2d)

## HTML-Validation-Job : 
![image](https://github.com/user-attachments/assets/1e00e871-dc5c-43f7-b0fb-75c1f7bbde18)

## Pipeline atelier 3 : 
![image](https://github.com/user-attachments/assets/e896058f-015d-430f-a93d-14ee5d993e98)





