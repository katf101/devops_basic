# Node 16을 base 이미지로 사용
FROM node:16 

# 컨테이너 상에서 app디렉토리로 전환
WORKDIR /app

# package.json 파일을 작업 디렉토리에 복사
COPY package.json .

# npm 설치
RUN npm install

# 나머지 코드 복사
COPY . .

# 컨테이너 내부뿐만 아니라 컨테이너 외부에서도 port300에 도달 가능
EXPOSE 3000

# node 명령으로 app.mjs 실행 가능
CMD [ "node", "app.mjs" ]