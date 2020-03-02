FROM ruby

EXPOSE 3000

RUN apt-get update && apt-get install -y \
    sqlite3 \
    libsqlite3-dev \
    nodejs

#install yarn    
RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add - && \
echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list && \
apt-get update && \
apt-get install -y yarn  
    
RUN gem install rails


WORKDIR /app
