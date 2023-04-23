# syntax=docker/dockerfile:1
# From means install image from docker hub like you have github projects
# WORKDIR / app means your file where ur project is the / when put move us to root 
# docker copy command is used to copy files to/from your docker container to the host file system. 

FROM node:18-alpine
WORKDIR /app
COPY . .
RUN yarn install --production
CMD ["node", "src/index.js"]
EXPOSE 3000