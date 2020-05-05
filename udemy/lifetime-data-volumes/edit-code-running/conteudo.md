https://jekyllrb.com/
Static site generator



# bindmount-sample-1
Servidor de página estática usando markdown


# comandos
cd bindmount-sample-1
docker run -p 80:4000 -v $(pwd):/site bretfisher/jekyll-serve
http://localhost:80
