FROM node:16.15.0
#boa prática colocar versão do sistema que está rodando, pois utilizar o latest pode gerar bugs
WORKDIR /app
COPY ./package*.json ./
RUN npm install
#Sempre copiar separado bibliotecas ou arquivos base/suporte que não serão alterados, assim otimiza na hora de criar a imagem
COPY . .
EXPOSE 8080
CMD ["node", "server.js"]