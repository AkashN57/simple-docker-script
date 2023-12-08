#1 Docker Build to create an image

docker build -t node-app:1.1 .

-t for tag 
node-app is the name of the image 
:1.1 tag of the image
. indicate current working directory 

#2 Docker Run to Build a container 
docker run -d -p 3000:3000 node-app:1.1

-d stands for detached (run in background)
-p 3000:3000 stands for publish (port to expose left one is host's port and right one is container's port)
node-app:1.1 is the name of the image with tag
