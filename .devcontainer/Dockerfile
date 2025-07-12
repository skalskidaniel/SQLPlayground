FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Update package lists and install SQLite3
RUN apt-get update && \
	apt-get install -y \
	sqlite3 \
	libsqlite3-dev \
	sqlite3-doc \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*

# Verify SQLite installation
RUN sqlite3 --version

# Create a workspace directory
RUN mkdir -p /workspace
WORKDIR /workspace

# Set the default user
USER vscode
