This is a simple programme to create a docker image and run it on docker containers. The programme simply prints out the version of numpy which was installed into the image, as declared in requirements.txt. 

To run this application, first trigger a builld of the image
```
docker build -t simple_app:1.0 .
```

Upon calling ```docker images```, you should see the entry to simple_app with TAG 1.0

Run the image by initiating a docker run
```
docker run simple_app:1.0
```

You should see the following prints
- <numpy installed version>
- Simple test app successful