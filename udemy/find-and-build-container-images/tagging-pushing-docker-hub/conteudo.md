Para esse exemplo precisa ter conta no hub.docker.com
e criar um repositório

# docker image tag
docker tag (old way)
assign one or more tags to an image

# docker image push
uploads changed layers to a image registr (default is Hub)

# docker login <server>
Defaults to logging in Hub, but you can override by adding server url.

# outros comando
docker login
docker logout



# comandos

docker image tag --help
docker image ls
docker pull mysql/mysql-server
docker image ls // repare a coluna REPOSITORY
docker pull nginx:mainline
docker image ls // vai aparecer mais um nginx


docker image tag nginx bretfisher/nginx
docker login
cat .docker/config
docker image push bretfisher/nginx
no hub.docker.com vai apare seu push
docker image tag nginx bretfisher/nginx bretfisher/nginx:testing
docker image ls
docker image push bretfisher/nginx:testing
vá no site e veja a nova image testing


