FROM node:16

RUN npm install -g http-server
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build
EXPOSE 8080
CMD ["http-server", "dist"]


# docker tag 454314925434.dkr.ecr.ap-northeast-1.amazonaws.com/ecs-sample-webapp:latest 454314925434.dkr.ecr.ap-northeast-1.amazonaws.com/ecs-sample-webapp:1.0.0