FROM python:latest

# Add user
RUN groupadd glot
RUN useradd -m -d /home/glot -g glot -s /bin/bash glot

# Install libs
RUN pip install \
    cachetools \
    nose \
    numpy \
    python-dateutil \
    pytz \
    six

# Copy files
COPY ./runner /home/glot/

USER glot
WORKDIR /home/glot/
