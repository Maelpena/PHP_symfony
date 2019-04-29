# Projet Symfony

Site web codé avec Symfony, creation, modification d'article, connection/deconnexion utilisateur, affichage d'un article en particulier, systeme de commentaire sur chaque article. utilisation d'une base de données Doctrine et affichage grâce à des templates Twig.

Cloner le projet, se rendre dans le dossier du projet avec un terminal et télécharger les dépendances : **composer install**

Editer le fichier .env pour recréer la BDD selon vos identifiants et le port d'accès à MySQL.  

DATABASE_URL=mysql://root:@127.0.0.1:8889/CRUD_symfony

Ensuite : 

- php bin/console doctrine:database:create
- php bin/console make:migration
- php bin/console doctrine:migrations:migrate

Si il y a une erreur avec la dernière commande, c'est normal car les tables existent déjà dans Migrations mais il faut quand même lancer la commande pour qu'elles existent vraiment dans PhpMyAdmin.

- php bin/console doctrine:fixtures:load


