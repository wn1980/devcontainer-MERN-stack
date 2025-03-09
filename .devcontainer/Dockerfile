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
RUN mkdir -p /home/node/.config && \
    chown node:node /home/node/.config && \
    mkdir -p /workspace && \
    chown node:node /workspace && \
    ln -sfn /workspace /home/node/workspace
    
