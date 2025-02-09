# FROM node:18-alpine
# FROM node:20-alpine
FROM node:22-alpine
RUN apk update && apk add --no-cache git
RUN npm install -g firebase-tools
COPY ./ngrok /usr/local/bin
COPY ./ngrok.yml /home/node/.config/ngrok/
RUN chmod 666 /home/node/.config/ngrok/ngrok.yml

# RUN addgroup -g 1000 developer && \
#     adduser -G developer -u 1000 developer -D
# USER developer
