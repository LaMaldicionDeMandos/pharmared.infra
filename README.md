# pharmared.infra
Archivos de infraestructura
#LANDING
## Creo el container
docker build --no-cache -t pharmared/home ./

##Corro la imagen y le pongo un nombre
docker run -d --name pharmared_landing pharmared/nginx

# NGINX
## Creo el contanedor de nginx
docker build --no-cache -t pharmared/nginx ./

## Corro la imagen
docker run -p 80:80 -p 443:443 -d --name pharmared_nginx pharmared/nginx
