# interop-docker
Repo for docker related code for modusbox images (dockerfile) and related code

Steps for building:

docker build -t modusbox/mule38java8 .
flags are in the dockerfile for changing java and mule versions

For running a dev container: 

docker run -d -v /opt/mule/logs:/opt/mule/logs -p 8081:8081 -p 8088:8088 -p 9081:9081 -p 9082:9082 --name devMule -e MULE_ENV=dev modusbox/mule38java8
