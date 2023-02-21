FROM node:latest

# set working directory
WORKDIR /



# update apt packages
# ARG env
# ENV APP_ENV=$env 
RUN echo 'we re in build docker file'
RUN npm install
RUN npm install -g typescript
COPY . /
RUN npm run build-ts

EXPOSE 80

CMD [ "node","./dist/index.js" ]
