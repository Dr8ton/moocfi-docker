#FRONTEND

FROM node:14

ENV NODE_ENV=production
ENV REACT_APP_BACKEND_URL="http://localhost:8080"

WORKDIR /usr/src/app

COPY ./material-applications/example-frontend/ .

RUN npm install --production
RUN npm install -g serve
RUN npm run build

EXPOSE 5000

CMD serve -s -l 5000 build


