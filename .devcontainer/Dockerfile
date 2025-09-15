FROM mcr.microsoft.com/devcontainers/go:1-1.24-bookworm

RUN apt-get update && apt-get install -y sqlite3 \
    && rm -rf /var/lib/apt/lists/*
