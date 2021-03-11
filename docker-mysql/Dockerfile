FROM golang:1.14
ENV SRC_DIR=/go/src/github.com/MudimukkuSreenath/
ENV GOBIN=/go/bin
WORKDIR $GOBIN
ADD . $SRC_DIR
RUN cd /go/src/;
RUN go get github.com/go-sql-driver/mysql;
RUN go get github.com/gorilla/mux;
RUN go install github.com/MudimukkuSreenath/;
ENTRYPOINT ["./MudimukkuSreenath"]
EXPOSE 8080