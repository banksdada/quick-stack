FROM node:22-alpine

ENV NODE_ENV=production

WORKDIR /app

COPY packages/ui/package*.json ./
RUN npm ci

COPY packages/ui ./

RUN npm run build

EXPOSE 3000

CMD ["npm", "start"]