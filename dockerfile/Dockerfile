FROM node:19.6-alpine3.16
RUN mkdir /devproject
WORKDIR /devproject
COPY /h/Devops/project/mydevproject/* /devproject
RUN npm install http-server -g
ENV API_URL=http://my-devproject.com
RUN cd /devproject; http-server
CMD npm start
