FROM ruby

RUN apt-get update

RUN apt-get install sqlite3

RUN apt-get -yq install nodejs

RUN apt-get -yq install wget

RUN wget https://raw.githubusercontent.com/rails/webpacker/master/lib/install/config/webpacker.yml

#COPY app/* /opt/app/


RUN gem install rails

RUN gem install bundler

WORKDIR /opt/

RUN rails new app


WORKDIR /

RUN mv webpacker.yml /opt/app/config

EXPOSE 3000
#RUN bundle install

WORKDIR /opt/app


#RUN rake db:migrate && rake db:seed




