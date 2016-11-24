## Jekyll-docker

It's a nice jekyll container better than [jekyll-docker](https://github.com/jekyll/docker)

## Usage

It just a base container.

you have to build your own container base on this container.

## Example

change your current dir to your jekyll project dir

and then edit your `Dockerfile` like this:

```bash
FROM annatarhe/jekyll:3.3.1
WORKDIR /jekyll
COPY Gemfile /jekyll/Gemfile
COPY Gemfile.lock /jekyll/Gemfile.lock
RUN bundle install
EXPOSE 4000
CMD ["bundle", "exec", "jekyll", "serve"]
```

and then run the `docker build .`

```bash
docker run -it -v /path/to/jekyll:/jekyll -p 4000:4000 your-own-jekyll-container
```

yes. here we go!

## NOTICE!!!

you have to add `host` column to your `_config.yml`

```yml
host 0.0.0.0
```
