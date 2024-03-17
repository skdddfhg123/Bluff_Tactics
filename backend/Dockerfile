FROM node:latest
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
ENV PORT=${NESTJS_PORT}
EXPOSE ${NESTJS_PORT}
CMD ["npm", "run", "start"]