FROM node:lts-alpine
WORKDIR /app
COPY package.json ./
RUN npm config set unsafe-perm true
RUN npm install --silent
RUN chown -R node /app/node_modules
USER node
EXPOSE 8081
CMD ["npm","run","serve","--","--port","8081"]


