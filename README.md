# api_rest_php
small rest app

# api_rest_php

0 Outil nécessaire pour tester cet api en local

1- installer un serveur local dans votre machine puis démmarer mysql et apache (utiliser laragon, wamp etc)

2- lancer phpmyadmin sur votre navigateur via cet address: http://localhost/phpmyadmin/index.php 

3- creer un utilisateur root sans mot de passe ou si vous disposer d'un autre user utiliser son user name et password 
pour configurer le fichier Connection disponible dans project/API/Config/connection.php; 

4-une fois phpmyadmin ouvert creer une bd nommé cancam

5-importer les table depuis le fichier cancam.sql present à la racine du projet

6-démarrer un terminal et pointer vers le dossier du projet taper la commande: php -S localhost:8000 (serveur interne propre à php)

7- rendez vous dans le navigateur à l'address: http://localhost:8000/

Autre remarque:

1-L'implementation android de cet api n'étant pas achever, les requetes en POST (http://localhost:8000/authenticate et http://localhost:8000/payment)
pourront néamoins etre tester en simulant le GET:

1-a   pour http://localhost:8000/authenticate ouvrer le dossier target du projet et se rendre sur authenticate.php; Décommenter la partie else de ce fichier pour
consulter les résultats json. 
2-b faire pareil pour payment via le fichier payment.php present dans target

Le fichier fill.php permettra de générer de nouveaux données dans la bd a condition de pointer l'invite de commande vers son 
dossier parent et taper: php fill.php




