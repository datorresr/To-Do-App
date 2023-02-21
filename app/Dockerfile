FROM node:12-alpine
RUN apk add --no-cache python2 g++ make
RUN apt-get update & apt-get install -y git
RUN mkdir /home/todoapp      
RUN cd /home/todoapp       
RUN git clone https://github.com/datorresr/To-Do-App.git
#Set working directory
WORKDIR /app
#WORKDIR /home/sampleTest
#COPY . .
RUN yarn install --production
CMD ["node", "src/index.js"]
EXPOSE 3000

