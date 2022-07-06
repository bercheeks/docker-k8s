FROM node:16-alpine as builder

WORKDIR /app

COPY package.json .
RUN npm install
COPY . .

RUN npm run build


#/app/build <----- all the stuff needed for prod

#second from statement means first block of docker is done
FROM nginx

#copy from first phase
COPY --from=builder /app/build /usr/share/nginx/html

#nginx automatically turns on