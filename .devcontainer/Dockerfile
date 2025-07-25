# syntax = devthefuture/dockerfile-x

FROM ../dev-support/docker/Dockerfile

ARG HOST_USER_ID
ARG HOST_USER_GID

ENV HOST_USER_ID=$HOST_USER_ID
ENV HOST_USER_GID=$HOST_USER_GID

RUN /user_mapping.sh

