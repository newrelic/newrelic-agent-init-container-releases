FROM ruby:latest

WORKDIR /app

COPY Gemfile ./

RUN bundle install

COPY . .

EXPOSE 9292

CMD ["bundle", "exec", "rackup", "--host", "0.0.0.0", "--port", "9292"]
 
# For local testing, run:
# curl http://0.0.0.0:9292
