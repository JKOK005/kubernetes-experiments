Docker build and run for a simple flask application

This project downloads the python 3 installation from docker, runs the necessary installations for flask as defined in requirements.txt and launches a container listening to a port. 

First initialize a build using

```
docker build -t setup-full-pip-installation:1.0 .
```

Launch the application using
```
docker run -d -p 5000:5080 setup-full-pip-installation:1.0 
```

A flask app should be ready for you to connect to via your host machine 

To see which port the container is listening to, do the following steps

```
# First get the container_id by listing all docker containers

docker ps

# Next see which port is being mapped from the container's port -> host port

docker port <container_id>
```

