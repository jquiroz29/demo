FROM node
# Define default ports and host for app and db
ARG app_port=3000

# Add dependencies for the node modules (to be installed)
COPY ["package.json", "package-lock.json", "/usr/src/"]

# Specify working directory for the container
WORKDIR /usr/src

# Install node dependencies via npm
RUN npm install

EXPOSE ${app_port}
CMD npm start
