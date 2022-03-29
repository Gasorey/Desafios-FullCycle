FROM golang:1.18 as builder

WORKDIR /usr/src/app

COPY go.mod go.sum ./
RUN go mod download

COPY . .

ENTRYPOINT [ "go" ]

CMD ["run main.go"]
