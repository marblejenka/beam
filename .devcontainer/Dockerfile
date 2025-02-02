FROM ghcr.io/marblejenka/devcontainers/beam:latest

ARG USERNAME=beam
ARG GROUPNAME=beam
ARG UID=1001
ARG GID=1001
RUN groupadd -g $GID $GROUPNAME && \
	useradd -m -s /bin/bash -u $UID -g $GID $USERNAME

RUN mkdir -p /workspaces && chown $USERNAME:$GROUPNAME /workspaces

USER beam
RUN ./gradlew :checkSetup
