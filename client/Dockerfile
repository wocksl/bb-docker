# node 19 베이스로 build 생성
FROM node:19

# 작업 디렉토리 설정
WORKDIR /app

# 애플리케이션 파일 복사
COPY . .

# Proxy 기능 설치
RUN npm install http-proxy-middleware

# 종속성 설치
RUN npm install

# 애플리케이션 실행
CMD ["npm", "run", "start"]

# 포트 노출
EXPOSE 3000

# # 애플리케이션 빌드
# RUN npm run build

# # nginx 베이스로 생성
# FROM nginx:alpine

# # nginx.conf 파일 복사
# COPY ./nginx.conf /etc/nginx/nginx.conf

# # 빌드 파일 복사
# COPY --from=build /app/build /usr/share/nginx/html

# # 포트 노출
# EXPOSE 3000

# # 애플리케이션 포어그라운드로 동작
# CMD ["nginx", "-g", "daemon off;"]