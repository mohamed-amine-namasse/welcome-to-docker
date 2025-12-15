*On se positionne dans le dossier welcome-to-docker
cd welcome-to-docker
![alt text](image.png)
*Créer l’image docker à partir de ce projet de sorte que le fichier dockerfile soit pris en compte
docker build -t mon-app-perso:1.0 .
![alt text](image-3.png)
![alt text](image-4.png)
*Lancer l’image docker que vous venez de créer et lancer un container avec
docker run -d --name mon-serveur-web -p 8080:3000 mon-app-perso:1.0
![alt text](image-5.png)
*Accéder au container pour visualiser le résultat
docker ps
![alt text](image-2.png)
![alt text](image-1.png)
