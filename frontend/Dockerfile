FROM node:14.17.3

WORKDIR /app/frontend
COPY package.json /app/frontend

RUN npm install
RUN npm install bootstrap jquery axios

EXPOSE 3000
CMD ["npm", "start"]