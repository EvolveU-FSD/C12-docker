## Getting Started

Assuming that you have Docker installed. If you do not have it installed yet please go [here](https://docs.docker.com/engine/install/)

at the root of the project run the following command to build the docker image:

`docker build -t next_docker:v1.0.1 . `

Note that the period needs to be a part of the command

The build may take a couple minutes, once completed you can check if the image is available with the command: 

`docker images`

this should show you the image you just created in the terminal output. once you confirm that you can start your container with the following command:

`docker run -p 3000:3000 next_docker:v1.0.1`

you should be able to access the app at localhost:3000

Note that changes to the file will require the image being rebuilt in order to see the change reflected in the application. alternatively you would have to access the file directly in the container