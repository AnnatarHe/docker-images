FROM golang:1.7.3
MAINTAINER AnnatarHe <iamhele1994@gmail.com>

ENV http_proxy http://h1.agent02.net:26324
ENV https_proxy http://h1.agent02.net:26324

RUN go get github.com/revel/cmd/revel
WORKDIR /go

CMD ["/bin/bash"]

