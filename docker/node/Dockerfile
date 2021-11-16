FROM node:16-alpine
WORKDIR /usr/src/app
COPY ./node/react-sample/ ./
RUN npm install -g npm \
&& npm install \
&& rm -rf /var/lib/apt/lists/*
RUN npm run build
CMD [ "npm", "run", "start" ]
EXPOSE 3000
