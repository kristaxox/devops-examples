FROM golang:1.11-alpine AS build-stage

COPY main.go /go/src/foo/
WORKDIR /go/src/foo

RUN go get -v ./...
RUN go build -o helloworld

FROM alpine
COPY --from=build-stage /go/src/foo/helloworld /opt/helloworld
ENTRYPOINT /opt/helloworld