# multi-container-docker
A Node.JS based and overly complicated fibonacci calculator to practice with docker

# Architecture:
<p align="center">
<img src="https://s3.us-west-2.amazonaws.com/secure.notion-static.com/c776f41f-dc9b-4837-8f0d-e51620d4b529/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5%2F20200711%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20200711T214658Z&X-Amz-Expires=86400&X-Amz-Signature=f5e274888cc4298bc3ead3a18b044a0df2eeae5c7b2e1f7e11935c84802525cc&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22">

</p>

# Production Flow

1. Push to Github
2. Travis builds test image and runs tests against it
3. Travis builds prod images
4. Travis pushes prod images to Docker Hub
5. Travis pushes project to AWS Elastic Beanstalk (EB)
6. EB pulls images from Docker Hub and deploys