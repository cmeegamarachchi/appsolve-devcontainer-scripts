FROM mcr.microsoft.com/devcontainers/python:2-3.14-trixie

ENV TZ=Australia/Perth

USER root

# Work around broken Yarn APT repository in upstream devcontainer image.
# Node is installed separately via the devcontainer Node feature.
RUN rm -f /etc/apt/sources.list.d/yarn.list \
    && rm -f /etc/apt/sources.list.d/yarn*.list

USER vscode