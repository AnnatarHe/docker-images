FROM golang:1.8.3
MAINTAINER AnnatarHe <iamhele1994@gmail.com>

ENV http_proxy http://your.agent.proxy:port
ENV https_proxy http://your.agent.proxy:port

RUN go get github.com/revel/cmd/revel
WORKDIR /go

CMD ["/bin/bash"]

