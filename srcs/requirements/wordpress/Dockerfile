FROM wordpress:latest

# Installer les utilitaires nécessaires
RUN apt-get update && apt-get install -y vim

# Modifier la configuration d'Apache pour écouter sur le port 9000
RUN sed -i 's/Listen 80/Listen 9000/' /etc/apache2/ports.conf
RUN sed -i 's/:80/:9000/' /etc/apache2/sites-available/000-default.conf

# Ajouter ServerName à la configuration principale d'Apache
RUN echo "ServerName ibenhaim.42.fr" >> /etc/apache2/apache2.conf

# Exposer le port 9000
EXPOSE 9000

# Démarrer Apache
CMD ["apache2-foreground"]
