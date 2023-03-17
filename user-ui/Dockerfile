FROM node:17.9.0-slim
LABEL maintainer="Avinash"
RUN useradd userui
WORKDIR /app
COPY . .
RUN npm install
RUN mkdir -p node_modules/.cache && chmod -R 777 node_modules/.cache
EXPOSE 3000
USER userui
CMD [ "npm","start" ]