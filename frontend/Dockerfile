FROM node:14.17.3

WORKDIR /src/app

ENV PATH /src/app/node_modules/.bin:$PATH

COPY package.json /src/app


RUN npm install
RUN npm install bootstrap jquery axios

EXPOSE 3000
CMD ["npm", "start"]