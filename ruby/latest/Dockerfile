FROM ruby:latest

# Add user
RUN groupadd glot
RUN useradd -m -d /home/glot -g glot -s /bin/bash glot

# Copy files
COPY ./runner /home/glot/

USER glot
WORKDIR /home/glot/
