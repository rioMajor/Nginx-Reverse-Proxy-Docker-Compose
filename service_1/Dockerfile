FROM golang:1.20-alpine

WORKDIR /app

COPY go.mod ./
RUN go mod tidy

COPY . .

RUN go build -o app

EXPOSE 8001

CMD ["./app"]
