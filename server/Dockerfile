FROM node

# set working directory
WORKDIR /

COPY . /

# update apt packages
ARG port
RUN npm install
RUN npm run build

EXPOSE 80

CMD [ "node","./dist/index.js" ]
