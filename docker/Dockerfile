# use an official Node.js runtime as  the base image
FROM node:21-alpine

# Set an workflow directory in th constainer
WORKDIR /usr/src/app

# Instal package.json and package-loack.json to the working directory
COPY package*.json ./

# Installl dependencies
RUN npm install

# Copy the rest of the application code to the working directory.
COPY . . 

# Expose the port on which your Node.js app runs
EXPOSE 3000

# Command to run your Node js app.  
CMD ["npm", "start"]