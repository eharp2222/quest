#base image
FROM node:18

#Create app directory
WORKDIR /home/ec2-user/quest-master

#Install app dependencies
#A wild card is used to ensure both package.json AND package-lock.json are copied
COPY package*.json ./

RUN npm install

#Bundle app source
COPY . .

#Create app directory
WORKDIR /home/ec2-user/quest-master

EXPOSE 3000

CMD [ "node", "000.js" ]
