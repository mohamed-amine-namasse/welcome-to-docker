## On lance docker-composer en arrière plan avec docker-compose up -d

![alt text](image-6.png)

## Accès à Adminer via l'URL http://localhost:8081 pour gérer la base de données

![alt text](image.png)

## On insére les bons infos

![alt text](image-1.png)

## Après authentification sur Adminer

![alt text](image-2.png)

## Accès au backend via l'URL http://localhost:3000

On voit bien le message de bienvenue

![alt text](image-3.png)

## Accès au frontend via l'URL http://localhost:8080 affichant l'état de l'API

![alt text](image-4.png)

## Accès à mysql via l'URL http://localhost:3306

On remarque qu'il ya une erreur
![alt text](image-5.png)

# Accès a la base de donnée par terminal

On tape la commande suivante pour entrer dans le conteneur et lancer mysql: docker exec -it mysql_db mysql -u root -p
![alt text](image-7.png)

Après on tape le mdp root et la commande SHOW DATABASES;
![alt text](image-8.png)

pour quitter on tape la commande exit;
![alt text](image-9.png)
