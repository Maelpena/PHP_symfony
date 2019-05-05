# Projet Symfony (projet est en cours et ne fonctionne pas correctement pour le moment)

Site web codé avec Symfony, creation/modification d'article, inscription/connexion/deconnexion d'utilisateur, affichage d'un article en particulier, systeme de commentaire sur chaque article. Utilisation d'une base de données avec Doctrine et affichage grâce à des templates Twig.


1- Cloner le projet, installer composer, se rendre dans le dossier du projet avec un terminal et télécharger les dépendances : **composer install**

2- Editer le fichier .env pour recréer la BDD selon vos identifiants et le port d'accès à MySQL :
        DATABASE_URL=mysql://root:@127.0.0.1:8889/CRUD_symfony

3- Ensuite, taper ces commandes dans l'invité de commande : 

- php bin/console doctrine:database:create
- php bin/console make:migration
- php bin/console doctrine:migrations:migrate

Si il y a une erreur avec la dernière commande, c'est normal car les tables existent déjà dans Migrations mais il faut quand même lancer la commande pour qu'elles existent vraiment dans PhpMyAdmin.

4- Et pour finir afin d'avoir les "fausses données" :
- php bin/console doctrine:fixtures:load


