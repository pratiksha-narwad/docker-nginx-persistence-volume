// persistent volume with nginx 

git clone https://github.com/atulkamble/docker-nginx-persistence-volume.git

cd docker-nginx-persistence-volume

sudo docker run -d -p 80:80 nginx

sudo docker volume create nginx_volume_test

docker volume ls 

docker container ls 
or 
docker ps -a

docker cp ./data/index.html 4b97ab275607:/usr/share/nginx/html/index.html

docker system prune -a

docker compose up --build 

docker compose down 