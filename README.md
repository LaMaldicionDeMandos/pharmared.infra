# pharmared.infra
Archivos de infraestructura

# NGINX
## Creo el contanedor de nginx
docker build --no-cache -t pharmared/nginx ./

## Corro la imagen
docker run -p 80:80 -p 443:443 -d pharmared/nginx
