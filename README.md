# devops-dockerlab
<font size = "5"> Docker a node.js app by writing your own Dockerfile. </font>

<font size = "3"> 1. Build the Docker image by running the following command  </font>
```
docker build -t devops-dockerlab .
```
<font size = "3"> 2. Run a Docker container with limits on CPU and memory by running the following command:  </font>
```
docker run -d -p 80:80 --name devops-dockerlab --cpus 0.5 --memory 512m devops-dockerlab
```
<font size = "3"> 3.Create a tag:  </font>
```
docker tag devops-dockerlab dstakhurskyi/devops-dockerlab
```
<font size = "3"> 4.Push Docker image to Docker Hub by running the following command:  </font>
```
docker push dstakhurskyi/devops-dockerlab
```

<font size = "5"> <b> Run a container from a pulled Docker image. </b> </font>

<font size = "3"> 1. Pull the Docker image from Docker Hub: </font>
```
docker pull dstakhurskyi/devops-dockerlab
```
<font size = "3"> 2. Pull Node: </font>
```
docker pull node
```
3. Run the container using the docker run command. Run the npm start command inside the container:
 ```
docker run -p 8080:80 devops-dockerlab npm start
```
4. Stop running container:
```
docker stop devops-dockerlab
```
