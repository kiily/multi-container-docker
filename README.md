# multi-container-docker
A Node.JS based and overly complicated fibonacci calculator to practice with docker

# Architecture:

![multi-container-docker](https://user-images.githubusercontent.com/22813414/87355189-d84d6980-c557-11ea-9870-2bd8eeed9bdf.png)

# Production Flow

1. Push to Github
2. Travis builds test image and runs tests against it
3. Travis builds prod images
4. Travis pushes prod images to Docker Hub
5. Travis pushes project to AWS Elastic Beanstalk (EB)
6. EB pulls images from Docker Hub and deploys
