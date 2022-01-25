FROM node:12

# Dejamos el package.json de primero porque si modificamos algo en el codigo y copiamos todo, todo se invalida y se vuelve a ejecutar todo lo de abajo
COPY ["package.json", "package-lock.json", "/usr/src/"]

WORKDIR /usr/src

RUN npm install

COPY [".", "/usr/src/"]

EXPOSE 3000

#CMD ["node", "index.js"]
#CMD ["npx", "nodemon", "index.js"]
