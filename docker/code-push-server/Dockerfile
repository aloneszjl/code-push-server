FROM node:8.11.4-alpine

RUN npm i -g https://github.com/aloneszjl/code-push-server.git pm2@latest --no-optional

COPY ./process.json /process.json

EXPOSE 3000

CMD ["pm2-docker", "start", "/process.json"]
