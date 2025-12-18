on construit l'image docker avec docker build -t
![alt text](image-10.png)
on la visualise sur navigateur sur le port 8080 apres avoir fait docker run
![alt text](image-5.png)
![alt text](image-2.png)
On crée un volume
docker volume create game-results
![alt text](image-3.png)
On liste les volumes on voit bien que le volume game-results a bien été créé
![alt text](image-4.png)
On relie le volume au conteneur
docker run -d -p 8080:80 -v game-results:/usr/share/nginx/html/data serveur-tic-tac-toe

![alt text](image-7.png)

On voit bien que les résultats s'enregistre bien dans le volume après une partie
![alt text](image-11.png)

la commande qui permet de voir à l'intérieur d'un conteneur
docker exec -it id_conteneur ls
![alt text](image-15.png)

la commande qui perment de voir à l'intérieur d'un volume
docker run --rm -v game-results:/donnees alpine ls
![alt text](image-13.png)
![alt text](image-14.png)
