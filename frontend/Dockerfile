# Node.js 이미지를 베이스로 사용
FROM node:latest
# 작업 디렉토리 설정
WORKDIR /app
# package.json 및 package-lock.json 복사
COPY package*.json ./
# 의존성 설치
RUN npm install
# 소스 코드 복사
COPY . .
# 포트 환경 변수 설정
ARG REACT_PORT
ENV PORT=${REACT_PORT}
# 포트 설정
EXPOSE ${REACT_PORT}
# 애플리케이션 실행 명령
CMD ["npm", "run", "dev"]