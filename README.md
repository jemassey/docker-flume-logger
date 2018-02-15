
## Build Instructions

    docker build -t flume .

## To run

    docker run -d \
      -e FLUME_AGENT_NAME=a1 \
      -e FLUME_CONF_FILE=/var/tmp/flume.conf \
      -p 44441:41414 \
      --name flume1 \
      flume

    docker run -d \
      -e FLUME_AGENT_NAME=a1 \
      -e FLUME_CONF_FILE=/var/tmp/flume.conf \
      -p 44442:41414 \
      --name flume2 \
      flume

      docker run -d \
        -e FLUME_AGENT_NAME=a1 \
        -e FLUME_CONF_FILE=/var/tmp/flume.conf \
        -p 44443:41414 \
        --name flume3 \
        flume
# docker-flume-logger
