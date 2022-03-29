FROM golang:1.18 as builder

WORKDIR /app

COPY . .

RUN go build

ENTRYPOINT [ "./go" ]

FROM scratch

COPY --from=builder  /app .

ENTRYPOINT [ "./go"]