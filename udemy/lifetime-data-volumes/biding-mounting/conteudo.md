# nginx-server/Dockerfile
cd nginx-server
docker container run -d --name nginx -p 80:80 -v $(pwd):/usr/share/nginx/html nginx
http://localhost:80

docker container run -d --name nginx2 -p 8080:80 nginx
http://localhost:8080/

docker container exec -it nginx bash
cd usr/share/nginx/html/
ls -la

No terminal do host execute
cd nginx-server
touch testme.txt
Volte no terminal do docker e execute
ls -la  // vai aparecer o arquivo criado

No terminal do host
cd nginx-server
echo "is it me you're looking for" > testme.txt
http://localhost:80/testme.txt
