
# Step 1: Choose a base image
FROM node:14 

RUN apt-get update


# Step 2: Set the working directory inside the container
WORKDIR /usr/src/app

# Step 3: Copy package.json and package-lock.json (if available)
COPY package*.json ./

# Step 4: Install dependencies
RUN npm install

# Step 5: Copy the rest of your app's code into the container
COPY . .

# Step 6: Expose the port the app will run on
EXPOSE 3000

# Step 7: Define the command to run your app, this command runs when he container is instantiated from the image 
CMD ["npm", "start"] 