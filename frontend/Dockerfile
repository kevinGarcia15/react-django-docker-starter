# pull the base image
FROM node:carbon

# set the working direction
WORKDIR /app

# install app dependencies
COPY ./frontend/package.json ./

COPY ./frontend/package-lock.json ./

RUN ls -al
RUN npm install

# add app
COPY ./frontend ./

# start app
CMD ["npm", "start"]