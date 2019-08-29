FROM    node

MAINTAINER      yngus4862@naver.com

RUN     apt-get -y update
RUN     apt-get -y install git-core

ENV     root    /root/.docker-images

RUN     mkdir -p ${root}
WORKDIR ${root}
RUN     git clone https://github.com/nyangnyangpunch/cheese
WORKDIR ${root}/cheese
RUN     npm install

EXPOSE  8888

CMD ["node", "app.js"]
