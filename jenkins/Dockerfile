FROM node:8.11.1-alpine

WORKDIR /var/jenkins_home/workspace/node_react/src

VOLUME [ "/var/jenkins_home/workspace/node_react/src" ]

RUN npm install -g nodemon

ENV NODE_ENV=development
ENV DATABASE=mongodb://mongodb:27017/playground
ENV PORT=3000

EXPOSE 3000

CMD [ "nodemon", "-L", "src/index.js" ]
