FROM node:16

WORKDIR /app

RUN npm install -g serve

COPY ./app /app

RUN npm install && npm run build

EXPOSE 5000

CMD ["serve", "-s", "-l", "5000", "build"]
