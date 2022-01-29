FROM node:16.13.1-alpine 
#not add as BUILD

WORKDIR /app/src

# install app dependencies
COPY package.json ./
COPY package-lock.json ./
RUN npm install

#RUN npm install react-scripts -g --silent
COPY . ./

#Despues de hacer el copy, puedes hacer el test, ya que ya existen los archivos
RUN npm test

#start app
CMD ["npm","start"]

EXPOSE 3000




