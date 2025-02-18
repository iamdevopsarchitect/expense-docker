FROM node:20
EXPOSE 8080
ENV DB_HOST="localhost" 
# before doing the above, name the container as mysql
RUN mkdir /opt/server
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install 
CMD ["node", "index.js"]
