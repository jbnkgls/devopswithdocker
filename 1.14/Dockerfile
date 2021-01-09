FROM ruby:2.6.0
WORKDIR /mydir
COPY . .
EXPOSE 3000
RUN apt update 
RUN apt install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN gem install bundler
RUN bundle install
RUN rails db:migrate
CMD ["/bin/bash"]