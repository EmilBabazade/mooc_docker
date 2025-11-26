FROM node:16

WORKDIR /app

RUN npm install -g serve

COPY ./app /app

ENV REACT_APP_BACKEND_URL=http://localhost:8080

RUN npm install && npm run build

EXPOSE 5000

CMD ["serve", "-s", "-l", "5000", "build"]
