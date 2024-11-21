FROM node

ENV NO_UPDATE_NOTIFIER=1

EXPOSE 3000
EXPOSE 5000

WORKDIR /app

ADD . .
RUN npm install --silent --loglevel=error

# Instalar o pacote npm-run-all globalmente
RUN npm install -g npm-run-all

CMD ["npm", "run", "exec"]
