# dockerNodeJsApp
Simple starter for Docker + NodeJS app with expressJS
```
git clone https://github.com/enghamzasalem/dockerNodeJsApp.git 
cd dockerNodeJsApp
docker build -t simple_node_app .
docker images
```
You should your image [simple_node_app] 
```
REPOSITORY                                       TAG                 IMAGE ID            CREATED             SIZE
simple_node_app                                  latest              0bcf80380338        7 minutes ago       908MB
```
let's run our image ..
```
docker run -d  -p 8050:9000 --name hakaspoll simple_node_app
docker ps
```
You should find you image like this :
```
CONTAINER ID        IMAGE                                            COMMAND                  CREATED             STATUS              PORTS                                                NAMES
4c3cbf282640        simple_node_app                                  "docker-entrypoint.s…"   5 seconds ago       Up 4 seconds        0.0.0.0:8050->9000/tcp        
```
Open localhost:8050 you should see blank page with "Hello World!"

