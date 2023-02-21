FROM node:12-alpine
RUN apk add --no-cache python2 g++ make git
RUN mkdir /home/todoapp
RUN cd /home/todoapp       
RUN git clone https://github.com/datorresr/To-Do-App.git
#Set working directory
WORKDIR ./To-do-App/app
RUN yarn install --production
CMD ["node", "src/index.js"]
EXPOSE 3000

