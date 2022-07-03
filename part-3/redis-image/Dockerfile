# Use an existing docker image as a base
FROM alpine


# Download and install a dependency
RUN apk add --update redis
#random instruction to install, for cache rebuild example
RUN apk add --update gcc


# Tell the image what to do when it starts as a container
CMD [ "redis-server" ]