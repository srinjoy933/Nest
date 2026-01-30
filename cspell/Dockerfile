FROM node:24.13.0-alpine3.23

WORKDIR /opt/node

COPY package.json pnpm-lock.yaml ./

RUN npm install -g pnpm && \
    pnpm install

WORKDIR /nest

ENTRYPOINT ["/opt/node/node_modules/.bin/cspell"]
