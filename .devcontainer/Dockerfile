# [Choice] Debian / Ubuntu version: debian-10, debian-9, ubuntu-20.04, ubuntu-18.04
ARG VARIANT=debian-10
FROM mcr.microsoft.com/vscode/devcontainers/base:0-${VARIANT}
WORKDIR /src

# [Optional] Uncomment this section to install additional OS packages you may want.
#
# RUN apk add --no-cache <your-package-list-here>

RUN sudo apt-get update -y && sudo apt-get install -y bats

RUN bash -c "$(curl -s https://raw.githubusercontent.com/tinydog-llc/exercism-cli-setup/main/install.sh)"
