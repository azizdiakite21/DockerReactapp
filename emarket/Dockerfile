# Utiliser une image de Node.js en tant que base
FROM node:14-alpine

# Définir le répertoire de travail dans le conteneur
WORKDIR /app

# Copier le package.json et le package-lock.json dans le conteneur
COPY package*.json ./

# Installer les dépendances de l'application
RUN npm install

# Copier les fichiers de l'application dans le conteneur
COPY . .

# Compiler l'application
RUN npm run build

# Exposer le port 80
EXPOSE 82

# Démarrer l'application
CMD ["npm", "start"]

