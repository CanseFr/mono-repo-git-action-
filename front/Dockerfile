# Utilise une version plus récente de Node.js
FROM node:18-alpine

# Définit le répertoire de travail dans le conteneur
WORKDIR /app

# Copie les fichiers de dépendances
COPY package.json ./

# Installe les dépendances
RUN npm install --silent && npm install react-scripts@3.4.1 -g --silent

# Copie tout le code de l'application
COPY . .

# Expose le port 3000 (si ton app tourne sur ce port)
EXPOSE 3000

# Démarre l'application
CMD ["npm", "start"]
