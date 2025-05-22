FROM node:21

WORKDIR /app

COPY . .

RUN npm cache clean --force

RUN npm install  --legacy-peer-deps

COPY .env.sample .env.local

EXPOSE 5173

CMD ["npm", "run", "dev", "--", "--host"]
