FROM node 

WORKDIR /app

COPY . /app
# or COPY . ./  as current workdir is set to /app

RUN npm install

EXPOSE 80 
# docker ports are internal to the container so we need to expose them to access from outside

CMD ["node", "server.js"]
