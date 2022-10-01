# Laravel

## 0. Installation d'un projet Laravel avec macOS

Avant d'installer pour la première fois Laravel, nous devons être sûr que notre PC possède bien tous les logiciels requis : PHP et Composer.
Tapez les commandes suivantes pour vérifier si PHP et Composer sont correctement installés : 
``` 
php --version
composer --version
```
## 1. Installation de PHP et Composer

###### Installation de Homebrew 

**Homebrew** est un gestionnaire de packages pour macOS. Il permet de facilement instaler de nombreux programmes. Pour l'installer, écrivez ces deux lignes de commande :
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew install wget
```

###### Installation de PHP
Pour installer **PHP** avec Homebrew : 
```
brew install homebrew/php/php71
```

###### Installation de Composer

Composer est le gestionnaire de dépendances de PHP. Il permet de télécharger des bibliothèques. Composer permet également de créer des projets Laravel et de télécharger le framework, ce qui nous intéresse. 
Pour installer Composer avec Homebrew, tapez la ligne de commande suivante : 
```
brew install homebrew/php/composer
``` 
## 2. Création du projet

Pour créer un projet, dirigez vous vers le dossier dans lequel vous voulez créer votre projet, par exemple le dossier Documents : 
```
cd Documents
``` 
Ensuite créons le projet : 
```
composer create-projet --prefer-dist laravel/laravel project
```
Le serveur web de PHP permet d'afficher son site web dans son navigateur. Il faudra le lancer à chaque fois que vous commencez à développer. Lançons la commande suivante pour nous diriger dans le dossier du projet, puis la deuxième commande afin de lancer le projet : 
```
cd project
php artisan serve
```
Le console vous affiche que tout est fonctionnel et que votre site est accessible sur https://127.0.0.1:8000
