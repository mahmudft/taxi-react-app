# pull official base image
FROM node:latest

# set working directory
WORKDIR /usr/src/app

# add `/usr/src/app/node_modules/.bin` to $PATH
ENV PATH /usr/src/app/node_modules/.bin:$PATH

# install app dependencies
COPY . .
# COPY yarn.lock .
RUN yarn install

ENTRYPOINT [ "yarn", "run", "start" ]
# copy project
