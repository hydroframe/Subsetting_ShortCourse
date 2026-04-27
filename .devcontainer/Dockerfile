# Use official Python dev container image
FROM mcr.microsoft.com/devcontainers/python:3.11

# Set working directory
WORKDIR /workspaces/${REPO_NAME}

# Copy requirements
COPY requirements.txt /tmp/requirements.txt

# Install Python dependencies
RUN pip install --upgrade pip \
    && pip install -r /tmp/requirements.txt \
    && pip install jupyter ipykernel

# Ensure the kernel is registered
RUN python -m ipykernel install --user --name python --display-name "short_course"
