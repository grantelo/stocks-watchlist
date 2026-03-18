ARG ALPINE_VERSION=3.23

FROM node:24-alpine${ALPINE_VERSION}

WORKDIR /app
COPY package*.json ./
RUN npm ci --only=production
COPY . ./
EXPOSE 3001 3002
CMD ["node", "index.js"]