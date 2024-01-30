# Dockerization

## Step 1
### First fork any github repository you want. we are forking javascript chat application
### github repo : https://github.com/Pragati0510/project_chat_application

![imagegit1](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/6f15b451-78b9-40c9-9803-adc9bc9753b4)

## Step2
### secondly copy https the code of the forked repository

![imagegit2](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/0893d065-d387-4512-b081-56770cbde2c5)

## Step 3
### Clone the git repository

```console
git clone <your_repository_url>
```

![image4](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/f4c2aa3c-9342-40d1-87c6-a23ad8255722)

## Step 4
### Now you have to create an application in your cloned project

```console
npx create-react-app myapp
```

## Step 5
### After your model has been now create a Dockerfile in your project directory
#### Note: rename your dockerfile as Dockerfile not Dockerfile.txt

![image](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/00772fef-7ac7-49ed-b815-e6b216cb7ff2)

## Step 6
### After your dockerfile has been created input some code in your dockerfile as related your project 
### Basic syntax of dockerfile

``` console
# Use an existing Docker image as a base
FROM base_image

# Set the working directory inside the container
WORKDIR /app

# Copy files or directories from the host machine to the container's filesystem
COPY source_path destination_path

# Run a command inside the container
RUN command

# Expose ports to allow communication with the container
EXPOSE port_number

# Define an environment variable
ENV key=value

# Start the main application process within the container
CMD ["command", "arg1", "arg2"]
```

## My project code

```console
FROM node:latest

# Set the working directory inside the container
WORKDIR /app
# Install nodemon globally
RUN npm install -g nodemon

# Copy both package.json and package-lock.json to the working directory
COPY ./client/src/App.js /app
COPY ./client/src/index.js /app
COPY ./client/package.json /app
COPY ./client/package-lock.json /app
COPY ./client/public/index.html /app
COPY ./server/package.json /app
COPY ./server/package-lock.json /app
COPY ./server/index.js /app
COPY ./server/router.js /app
COPY ./server/users.js /app

# Install project dependencies
RUN npm install 


# Copy the rest of the application code
COPY . /app

# Expose any ports the app needs
EXPOSE 5000

# Define the command to run the application
CMD [ "npm", "start" ]
```
#### Note :code can be like this but have to make some changes according to your project 

## Step 6
### Building a docker image 
#### Note: you have to download the base image of any technology or language which is used in your project

#### code for making an image of a project

```console
docker build -t your-image-name .
```

![image](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/025a2a62-a22c-4898-bfe9-c7928b303551)

#### after this your image will be visible in your docker desktop

![image](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/50d8082e-8ad8-43e7-ab0f-d6da576be506)

## Step 7
### Building a container with an image

##### just run that image with a specified container_name and port address

![image](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/3e47edb0-76bb-41e0-b450-ce148e744bbb)

#### After your container has been successfully running without any errors you can go to localhost address and can run that you will seee that your project has been running successfully

![image](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/0a1dbadc-bbef-4fd1-901c-27681d78a41d)



