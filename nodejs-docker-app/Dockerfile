FROM node:10

# working directory
# 컨테이너에 올릴 때 파일들의 경로를 지정해주는 것
WORKDIR /usr/src/app

# 소스 파일 복사
COPY package.json ./

RUN npm install

# 캐시를 이용하도록 하는 것
COPY ./ ./

CMD ["node", "server.js"]