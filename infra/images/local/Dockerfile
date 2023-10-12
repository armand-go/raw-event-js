FROM node:20

WORKDIR /usr/src/app

COPY package.json ./
COPY yarn.lock ./

RUN yarn install

COPY . .

ENV NODE_ENV dev

RUN mkdir /home/node/commandhistory && touch /home/node/commandhistory/.zsh_history

# # Install application into container
# COPY . /home/dashboard
# COPY ./infra/images/local/.zshrc /home/node/.zshrc
# COPY ./infra/images/local/entrypoint.sh /bin/entrypoint

# ENV SHELL /bin/zsh

# ENTRYPOINT ["entrypoint"]

