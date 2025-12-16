On se met dans le dossier welcome-to-docker et on tape docker pull pengbai/docker-supermario
![alt text](image.png)
![alt text](image-2.png)
On remarque que l'image mario a bien été ajouté
![alt text](image-1.png)

On lance l'image sur le port 8600 en considérant que l’image est configuré sur le port 8080 et on visualise sur navigateur
![alt text](image-3.png)
![alt text](image-4.png)
On peut egalement demarrer le conteneur manuellement on cliquant sur start
![alt text](image-5.png)
![alt text](image-6.png)

On lance le jeu sur un autre port 8800 par exemple
![alt text](image-11.png)
![alt text](image-7.png)
![alt text](image-8.png)
![alt text](image-9.png)
![alt text](image-10.png)
Pour trouver l'id du conteneur a arreter on fait docker ps qui afficher les conteneurs en cours d'execution
ou on le voit directement sur docker desktop
![alt text](image-15.png)
![alt text](image-14.png)

Pour supprimer le conteneur deux manières soit manuellement en cliquant sur delete ou à l'aide de la commande
docker stop puis docker rm
![alt text](image-12.png)
On voit bien que le conteneur avec le port 8800 a bien été supprimé
![alt text](image-13.png)

pour supprimer l'image docker images puis docker rmi -f id_image ou manuellement en cliquant sur delete sur images de docker desktop
![alt text](image-16.png)
![alt text](image-17.png)
on voit bien que l'image n'existe plus
![alt text](image-18.png)
![alt text](image-19.png)
