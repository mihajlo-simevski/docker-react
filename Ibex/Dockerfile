FROM node:alpine 
WORKDIR /Ibex

# COPY the package.json file, update any deps and install them
COPY package.json .
RUN npm update
RUN npm install

# copy the whole source folder(the dir is relative to the Dockerfile
COPY . .

CMD ["gatsby", "develop", "-H", "0.0.0.0" ]