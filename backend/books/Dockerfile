FROM golang:1.18.7-bullseye

WORKDIR /app

COPY go.mod ./
COPY go.sum ./

RUN go mod download

COPY *.go ./

RUN go build -o /app/books-api

EXPOSE 8080

CMD [ "/app/books-api"]