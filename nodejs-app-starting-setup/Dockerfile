FROM node 

WORKDIR /app

COPY package.json /app
# doing this will not run npm install each time we change our source code
RUN npm install

COPY . /app
# or COPY . ./  as current workdir is set to /app

EXPOSE 80 
# docker ports are internal to the container so we need to expose them to access from outside
# but this step is mostly used for documentation purpose

CMD ["node", "server.js"]
