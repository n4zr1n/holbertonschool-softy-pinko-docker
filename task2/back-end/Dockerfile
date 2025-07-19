# Use the latest Ubuntu image
FROM ubuntu:latest

# Prevent interactive prompts
ENV DEBIAN_FRONTEND=noninteractive

# Update and upgrade packages
RUN apt-get update && apt-get upgrade -y

# Install Python3 and pip
RUN apt-get install -y python3 python3-pip

# Fix pip installation error (if needed)
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip3
RUN pip3 install flask

# Set the working directory to /app
WORKDIR /app

# Copy the Flask app into the image
COPY ./api.py /app/api.py

# Run the Flask app
CMD ["python3", "api.py"]
