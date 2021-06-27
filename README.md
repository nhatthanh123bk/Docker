### Command to build entire services inside .yml file simultaneously.
```console
docker-compose build
```
  - You can add --no-cache option to void running everything kept in cache again
### Command to build specific services in .yml file
```console
docker-compose build service1 service2
```
### Command to create containers
```console
docker-compose up ID_Containers -d
```  
- option -d help you to run containers in the background 
### Command to stop container
``` 
docker-compose stop ID_Containers
```
or 
```
docker stop ID_Containers 
```
### Command to delete the Containers stopped.
```
docker container rm ID_Containers
```
- In order to delete whole containers stopped:
```
docker rmi $(docker images -q)
```
