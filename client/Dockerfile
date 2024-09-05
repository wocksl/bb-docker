FROM node:18 

WORKDIR /app

COPY . .

RUN yarn install

RUN yarn add @testing-library/dom
RUN yarn add @babel/plugin-syntax-flow@^7.14.5
RUN yarn add @babel/plugin-transform-react-jsx@^7.14.9
RUN yarn add typescript

EXPOSE 3000