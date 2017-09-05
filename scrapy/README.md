## Scrapy

a docker image build with scrapy, redis and postgres

so, you can do this with this image:

```python3
import psycopg2
import redis
import scrapy
```

## Usage

```shell
$ docker run -it -v ~/code/python:/py annatarhe/scrapy:v0.1 /bin/bash
```