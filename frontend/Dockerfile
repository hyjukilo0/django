FROM node:14.17.3

WORKDIR /src/app

ENV PATH /src/app/node_modules/.bin:$PATH

COPY package.json /src/app
COPY package_lock.json /src/app

RUN npm install
RUN npm install bootstrap jquery axios

COPY . .

EXPOSE 3000
CMD ["npm", "start"]