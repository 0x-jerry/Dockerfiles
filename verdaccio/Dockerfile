FROM arm32v7/node:12.16.2-alpine

RUN npm install --global verdaccio --registry=https://registry.npm.taobao.org/

EXPOSE $VERDACCIO_PORT

CMD verdaccio --config /verdaccio/conf/config.yaml --listen $VERDACCIO_PROTOCOL://0.0.0.0:$VERDACCIO_PORT