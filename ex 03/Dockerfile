FROM node

WORKDIR /app

# node.js 에서 package.json을 먼저 app폴더에 copy 하고
COPY package.json /app

# npm install을 한 후에
RUN npm install

# 모든 파일을 /app 에 다시 copy하면 image build 시 최적화 가능
COPY . /app

EXPOSE 80

CMD ["node", "server.js"]