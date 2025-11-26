FROM golang:1.16

WORKDIR /app

COPY ./app .

ENV REQUEST_ORIGIN=http://localhost:5000

RUN go build

ENV PORT=8080

EXPOSE 8080

CMD ["./server"]
