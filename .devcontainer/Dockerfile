#FROM node:18-alpine
#FROM node:20-alpine
FROM node:22-alpine
RUN apk update && apk add --no-cache git
RUN npm install -g firebase-tools && \
    npm install -g typescript
COPY ./ngrok /usr/local/bin
COPY ./ngrok.yml /home/node/.config/ngrok/
RUN chown -R  node:node /home/node/.config

# RUN addgroup -g 1000 developer && \
#     adduser -G developer -u 1000 developer -D
# USER developer
