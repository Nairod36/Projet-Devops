# Utiliser une image de base adaptée à votre application front-end (par exemple, Node.js)
FROM node:14 as backend

# Définir le répertoire de travail
WORKDIR /app

# Copier les fichiers nécessaires pour l'installation des dépendances
COPY package*.json ./

# Installer les dépendances
RUN npm install

# Copier le reste des fichiers de l'application front-end
COPY . .

# Exposer le port sur lequel votre application front-end écoute
EXPOSE 8080

# Commande pour lancer l'application front-end en mode développement
CMD ["npm", "run", "start"]
