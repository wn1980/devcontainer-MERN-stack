#FROM node:18-alpine
#FROM node:20-alpine
FROM node:22-alpine
RUN apk update && apk --no-cache add \
    git \
    curl
RUN npm install -g firebase-tools && \
    npm install -g typescript
RUN curl -O https://bin.equinox.io/c/bNyj1mQVY4c/ngrok-v3-stable-linux-amd64.tgz && \
    tar -xvzf ./ngrok-v3-stable-linux-amd64.tgz -C /usr/local/bin && \
    ngrok --version 
    
# && \
# chown -R  node:node /home/node/.config
# COPY ./ngrok /usr/local/bin
# COPY ./ngrok.yml /home/node/.config/ngrok/
# RUN chown -R  node:node /home/node/.config
# RUN addgroup -g 1000 developer && \
#     adduser -G developer -u 1000 developer -D
# USER developer
