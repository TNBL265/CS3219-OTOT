FROM node:18.8.0
ENV NODE_ENV=production

# create app directory
WORKDIR /app

# install deps
COPY package*.json .
COPY yarn.lock* .
RUN yarn install --prod

# copy source files
COPY . .

# run app
CMD ["yarn", "start"]