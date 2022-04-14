# syntax=docker/dockerfile:1
FROM node:12.18.1
ENV NODE_ENV=production
WORKDIR ~/app/
RUN find * -type d -name app
COPY ~/app/package.json /
COPY ~/app/package-lock.json /
RUN npm install --production
COPY . .
CMD [ "node", "server.js" ]

