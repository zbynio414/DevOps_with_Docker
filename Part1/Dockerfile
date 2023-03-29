FROM ubuntu:20.04

# install curl
RUN apt-get update && apt-get -y upgrade && apt-get -y install curl 

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Copy the hello.sh file from this location to /usr/src/app/ creating /usr/src/app/hello.sh
COPY curl.sh .
RUN chmod +x curl.sh

# When running docker run the command will be ./curl.sh
CMD ./curl.sh
