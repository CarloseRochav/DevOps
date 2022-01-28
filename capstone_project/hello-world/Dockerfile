FROM node:16.13.1-alpine 
#not add as BUILD

WORKDIR /app/src

# install app dependencies
COPY package.json ./
COPY package-lock.json ./
RUN npm install 
#RUN npm install react-scripts -g --silent

COPY . ./

#start app
CMD ["npm","start"]

EXPOSE 3000




