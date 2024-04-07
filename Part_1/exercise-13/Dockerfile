FROM golang:1.16-alpine

ENV PORT=8080
# ENV REQUEST_ORIGIN=https://example.com

EXPOSE 8080

WORKDIR /usr/src/app

COPY . .

RUN go build

CMD [ "./server" ]