FROM node:14.14.0-alpine

RUN mkdir -p /home/node/app
WORKDIR /home/node/app
COPY ./package.json ./
RUN npm install
COPY --chown=node:node ./ ./
CMD ["npm", "run", "start"]