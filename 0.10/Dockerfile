FROM buildpack-deps:jessie

ENV NPM_CONFIG_LOGLEVEL info
ENV NODEJS_VERSION 0.10.40

RUN curl -SLO "https://nodejs.org/dist/v$NODEJS_VERSION/node-v$NODEJS_VERSION-linux-x64.tar.gz" \
  && tar -xzf "node-v$NODEJS_VERSION-linux-x64.tar.gz" -C /usr/local --strip-components=1 \
  && rm "node-v$NODEJS_VERSION-linux-x64.tar.gz"

CMD ["nodejs"]
