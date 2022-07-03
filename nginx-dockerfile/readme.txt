## here we build image from docker file 
##n.b here we need to create a index.html file on current directory

docker build -t web . 

##check new images

docker images

##run container using build image

docker run --name webserver -dit  -p 8086:80 web
