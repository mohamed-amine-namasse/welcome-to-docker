# Utiliser l'image de base Nginx
FROM nginx:alpine

# Copier les fichiers dans le répertoire par défaut d'Nginx
COPY index.html /usr/share/nginx/html/index.html
COPY save.php /usr/share/nginx/html/save.php
COPY results.json /usr/share/nginx/html/results.json

# Exposer le port 80
EXPOSE 80