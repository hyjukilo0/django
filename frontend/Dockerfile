FROM node:14.17.3

RUN mkdir /frontend
WORKDIR /frontend/

ENV PATH /frontend/node_modules/ .bin:$PATH

COPY package.json /frontend/
COPY package_lock.json /frontend/

RUN npm install
RUN npm install bootstrap jquery axios

COPY . .

EXPOSE 3000
CMD ["npm", "start"]