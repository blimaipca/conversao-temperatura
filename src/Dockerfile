#1º indicar a imagem base
FROM node:16-alpine3.11
#Determinar o Workdir (diretorio de trab)
WORKDIR /app
COPY package*.json ./
#indicar os comandos para criar o container, indicar os pacotes a instalar
#assim benificia do Cache
RUN npm install
#A ideia é benificar da
COPY . .
EXPOSE 8080
CMD ["node","server.js"]

#docker image build -t brunotslima/conversao-temperatura:v1 . (push para o docker hub)
#docker container run -d -p 8080:8080 brunotslima/conversao-temperatura:v1