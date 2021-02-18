FROM ubuntu:20.04

RUN apt-get -y update &&\
    apt-get -y upgrade &&\
    apt-get install -y curl &&\
    curl -fsSL https://deb.nodesource.com/setup_14.x | bash - &&\
    apt-get install -y sqlite3 nodejs &&\
    mkdir /root/workspace &&\
    npm install -g @vue/cli

WORKDIR /root/workspace

RUN npm install

CMD ["/bin/bash"]
