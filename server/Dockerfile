FROM node:14.14.0-alpine

WORKDIR "/app"
COPY ./package.json ./
RUN npm install
COPY . .

RUN chown -R node:node /app/node_modules

USER node
CMD [ "npm", "run", "start" ]