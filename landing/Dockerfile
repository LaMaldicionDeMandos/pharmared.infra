FROM node:argon
MAINTAINER Marcelo Pasut pasutmarcelo@gmail.com
# Clone our private GitHub Repository
RUN apt-get install git
RUN git clone https://7fad9529ea239416c61bf94dc6dfa97b05f66143:x-oauth-basic@github.com/LaMaldicionDeMandos/pharmared.git /app/
RUN mkdir -p /home/app
RUN cp -R /app/* /home/app
WORKDIR /home/app
RUN npm install
EXPOSE 5000
CMD [ "npm", "start" ]
