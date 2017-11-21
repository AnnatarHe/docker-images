# annatarhe/revel:v0.18.0
FROM golang:1.9.2
MAINTAINER AnnatarHe <iamhele1994@gmail.com>

ENV GOROOT /usr/local/go
ENV GOPATH /go
ENV PATH $PATH:/usr/local/bin:/go/bin

ENV http_proxy http://10.9.13.83:1087
ENV https_proxy http://10.9.13.83:1087

RUN go get github.com/revel/cmd/revel
RUN go get github.com/revel/revel

# export http_proxy=http://127.0.0.1:1087;export https_proxy=http://127.0.0.1:1087;
ENV http_proxy ''
ENV https_proxy ''

WORKDIR /go

CMD ["/bin/bash"]

