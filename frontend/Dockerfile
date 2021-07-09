FROM node:14.17.3

WORKDIR /app/frontend/

ENV PATH /app/frontend/node_modules/ .bin:$PATH

COPY package.json /app/frontend/
COPY package_lock.json /app/frontend/

RUN npm install
RUN npm install bootstrap jquery axios

COPY . .

EXPOSE 3000
CMD ["npm", "start"]