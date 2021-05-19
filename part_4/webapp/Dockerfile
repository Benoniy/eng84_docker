FROM ubuntu:16.04
# First line of our Dockerfile

RUN apt-get update -y
RUN apt-get upgrade -y
RUN apt-get install npm -y

RUN apt-get install curl -y
RUN apt-get install python-software-properties -y
RUN curl -sL https://deb.nodesource.com/setup_6.x | bash -
RUN apt-get install nodejs -y

WORKDIR /home/ubuntu/app

COPY ./app .

RUN npm install -g pm2

RUN npm install

EXPOSE 3000

RUN echo "DB_HOST=mongodb://mongo:27017/posts" >> ~/.bashrc

CMD ["node", "app.js"]
