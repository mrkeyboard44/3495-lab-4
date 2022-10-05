FROM node:current-slim

# Copy source code to /src in container

RUN apt-get update
RUN apt install git -y
RUN git clone https://github.com/mrkeyboard44/3495-lab-4.git
RUN mv 3495-lab-4/App/ /src
RUN cd /src; npm install

# Document the port the app listens on
EXPOSE 8080

# Run this command (starts the app) when the container starts
CMD cd /src && node ./app.js
