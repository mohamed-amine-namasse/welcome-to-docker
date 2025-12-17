# Utilisation d'une image PHP avec Apache 
FROM php:8.2-apache

# Définir le répertoire de travail
WORKDIR /var/www/html

# Copier le fichier de jeu
COPY index.html .

# Créer le répertoire pour les données et copier les fichiers de sauvegarde
COPY save.php .
COPY results.json .

# Donner les permissions d'écriture pour que PHP puisse modifier results.json
RUN chown -R www-data:www-data /var/www/html && chmod -R 755 /var/www/html

# Exposer le port 80
EXPOSE 80