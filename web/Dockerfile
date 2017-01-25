FROM jruby:9.1-jdk 

RUN mkdir /app

WORKDIR /app

COPY Gemfile* /app/
RUN bundle install

COPY . /app/

RUN gem install warbler -v "2.0.4"

RUN warble
