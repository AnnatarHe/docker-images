FROM python:3
MAINTAINER AnnatarHe <iamhele1994@gmail.com>

ENV http_proxy http://10.9.13.137:1087
ENV https_proxy http://10.9.13.137:1087

RUN pip install scrapy redis psycopg2
RUN pip install scrapy-random-useragent

ENV http_proxy ''
ENV https_proxy ''

WORKDIR /py

CMD ["/bin/bash"]
