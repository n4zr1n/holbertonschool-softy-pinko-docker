# Use latest Ubuntu image
FROM ubuntu:latest

# Prevents user interaction during build
ARG DEBIAN_FRONTEND=noninteractive

# Update APT and upgrade installed packages
RUN apt-get update && apt-get upgrade -y

# Set command to echo Hello, World!
CMD ["echo", "Hello, World!"]
