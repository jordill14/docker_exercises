a.

Hago pull de la imagen:

docker pull nginx:1.19.3



Creo el index.html en la carpeta "html" en mi local:

echo "HOMEWORK" > index.html 

Creo el index.html, el Dockerfile y hago el build en la carpteta que tengo el Dockerfile:

docker build -t nginx:1.19.3 .

Arranco el contenedor con la imagen en el puerto 8080:

docker run -d -p 8080:80 nginx:1.19.3

Creo el docker volume:

docker create volume static_content

Y arranco un container mapeando el volumen:

docker run -it -d --rm -p 8080:80 -v static_content:/usr/share/nginx/html nginx:1.19.3

lo paro, y arranco otro container con otra versión de nginx y miro si el archivo persiste:

docker run -it -d --rm -p 8080:80 -v static_content:/usr/share/nginx/html nginx






docker run -d --name demo -p 8080:80 nginx:1.19.3

docker exec -it demo sh

cd /usr/share/nginx/html
echo "HOMEWORK 1" > index.html
exit




docker volume create static_content

docker container run -it --rm -v static_content:/demo nginx:1.19.3