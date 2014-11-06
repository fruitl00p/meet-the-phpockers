# A simple docker file as a demo @ see http://docs.docker.com/examples/running_redis_service/
FROM        ubuntu:14.04
RUN         apt-get update && apt-get install -y redis-server
EXPOSE      6379
ENTRYPOINT  ["/usr/bin/redis-server"]
