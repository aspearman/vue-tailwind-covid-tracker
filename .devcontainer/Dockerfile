# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.192.0/containers/typescript-node/.devcontainer/base.Dockerfile

ARG VARIANT="16-buster"
FROM mcr.microsoft.com/vscode/devcontainers/typescript-node:0-${VARIANT}

RUN su node -c "npm install -g @vue/cli"
