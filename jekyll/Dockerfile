FROM ruby:2.3.3
MAINTAINER AnnatarHe <iamhele1994@gmail.com>

RUN gem sources --add https://gems.ruby-china.org/ --remove https://rubygems.org/
RUN gem install jekyll bundler
RUN bundle config mirror.https://rubygems.org https://gems.ruby-china.org

RUN mkdir /jekyll
RUN chmod -R 777 /jekyll
WORKDIR /jekyll

RUN bundle install

CMD ["bundle", "exec", "jekyll", "serve"]

