# Utiliser l'image de base Nginx
FROM nginx:latest
# copier fichier conf
COPY nginx.conf /etc/nginx/conf.d/default.conf
#installer php
RUN apt-get update && apt-get install -y php-cli php-cgi
# Copier les fichiers dans le répertoire par défaut d'Nginx
COPY index.html /usr/share/nginx/html/index.html
COPY save.php /usr/share/nginx/html/save.php
COPY results.json /usr/share/nginx/html/results.json
# Donner les permissions d'écriture pour que PHP puisse modifier results.json
RUN chown -R www-data:www-data /usr/share/nginx/html && chmod -R 755 /usr/share/nginx/html
# Instruction pour indiquer que ce chemin peut être un volume
VOLUME /usr/share/nginx/html

# Exposer le port 80
EXPOSE 80
# lancer les deux services nginx et php

CMD ["sh", "-c", "php-cgi -b 127.0.0.1:9000 & nginx -g 'daemon off;'"]