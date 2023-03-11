# Lab#3
## Building a Node.js App with Docker

### student - Daria Shmielova

####1) build the image
docker build -t darshm21/app .

####2) to push the image to the repository, create a tag for the image
docker tag darshm21/app darshm21/app:lab3          

####3) check an availiability of the image you created
docker images

####4) push the image to the repository
docker image push darshm21/app:lab3     

####5) run the app in the container daria-container
docker run --memory=1g --cpus=2 --name daria-container darshm21/app:lab3
