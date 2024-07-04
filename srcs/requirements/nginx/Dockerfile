# Utiliser l'image de base NGINX depuis le registre Docker Hub
FROM nginx:alpine

# Copier le fichier de configuration NGINX dans le répertoire de configuration de NGINX dans le container
COPY conf/nginx.conf /etc/nginx/nginx.conf

# Copier les certificats SSL
COPY certs/nginx-selfsigned.crt /etc/ssl/certs/
COPY certs/nginx-selfsigned.key /etc/ssl/private/

# Exposer le port 443 pour HTTPS
EXPOSE 443
