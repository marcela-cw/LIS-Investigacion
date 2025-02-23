#usar imagen de Node.js como base
FROM node:22-alpine

# directorio de trabajo del contenedor
WORKDIR /app

#copiar package.json y package-lock.json al contenedor
COPY package*.json ./

#instalar las dependencias
RUN npm install

#copiar el resto del código al contenedor
COPY . .

#puerto en el que se ejecutara la API
EXPOSE 3000

#comando para iniciar la app
CMD ["node","server.js"]