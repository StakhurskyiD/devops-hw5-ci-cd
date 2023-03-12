# devops-dockerlab
Docker a node.js app by writing your own Dockerfile.
# 1. Build the Docker image by running the following command
docker build -t devops-dockerlab .
# 2. Run a Docker container with limits on CPU and memory by running the following command:
docker run -d -p 80:80 --name my-node-app --cpus 0.5 --memory 512m my-node-app
# 3.
# 4.Push your Docker image to Docker Hub by running the following command:
docker tag devops-dockerlab dstakhurskyi/devops-dockerlab
docker push dstakhurskyi/devops-dockerlab
# 5.
