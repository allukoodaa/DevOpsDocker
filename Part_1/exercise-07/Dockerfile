# Start from the ubuntu image
FROM ubuntu:22.04

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Install curl into image
RUN apt-get update && apt-get install -y curl

# Copy the script from this location to /usr/src/app/ creating /usr/src/app/hello.sh.
COPY script.sh .

# Give permission to execute, uncomment if permission denied during build
# RUN chmod +x script.sh

# Run script on container start
CMD ./script.sh