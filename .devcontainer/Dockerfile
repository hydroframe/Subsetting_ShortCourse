# Use official Python dev container image
FROM mcr.microsoft.com/devcontainers/python:3.11

# Set working directory
WORKDIR /workspaces

# Copy requirements
COPY requirements.txt /tmp/requirements.txt

# Install Python dependencies
RUN pip install --upgrade pip \
    && pip install -r /tmp/requirements.txt
