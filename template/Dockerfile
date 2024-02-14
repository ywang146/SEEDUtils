# Set the values for below args as per your environment

# Example: python, ubuntu, alpine
ARG BASE_IMAGE=python
 # Example: Python version (3.9, 3.9-slim)
ARG TAG=3.9
# Example: Your projects source directory default .
ARG SOURCE_DIR=.
# Example: Working directory inside the container default:/app
ARG DEST_DIR=/app 
# Example: Main script to execute
ARG SCRIPT_FILE=main.py 



# Specify base image using build-time variable
FROM ${BASE_IMAGE}:${TAG}

# Set working directory using build-time variable
WORKDIR ${DEST_DIR}

# Copy requirements.txt for efficient caching
COPY requirements.txt requirements.txt

# Install dependencies
RUN pip install -r requirements.txt

# Copy project code using source directory variable
COPY ${SOURCE_DIR} .

# Placeholder for additional configuration steps specific to contributor's code

# Set default command to start the application
# Enclose script file in double quotes
CMD ["python", "${SCRIPT_FILE}"] 