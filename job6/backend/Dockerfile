FROM node:16-alpine

WORKDIR /app

# On copie d'abord les fichiers de dépendances
COPY package*.json ./

# On installe les dépendances (express et mysql2)
RUN npm install express mysql2

# On copie le reste du code source
COPY . .


EXPOSE 3000
CMD ["node", "server.js"]




