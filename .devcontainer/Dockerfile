FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

RUN apt-get update \
 && apt-get install -y --no-install-recommends curl unzip \
 && curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o /tmp/awscliv2.zip \
 && unzip -q /tmp/awscliv2.zip -d /tmp \
 && /tmp/aws/install --update \
 && rm -rf /tmp/aws /tmp/awscliv2.zip \
 && apt-get clean \
 && rm -rf /var/lib/apt/lists/*
