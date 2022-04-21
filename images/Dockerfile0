FROM node:14

# Create app directory
WORKDIR /usr

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)


RUN npm install -g @angular/cli
RUN ng new angularTest
WORKDIR /usr/angularTest
RUN ng build

EXPOSE 8080
CMD [ "ng", "serve", "--host", "0.0.0.0", "--port", "8080" ]
