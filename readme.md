Copy from nginxx
docker cp nginx-base-test:/etc/nginx/conf.d/default.conf /Users/madhusudantripathy/Documents/DockerProjects/reverse-proxy-test/ReverseProxy/default.conf

make your changes

sent it back to nginx
docker cp /Users/madhusudantripathy/Documents/DockerProjects/reverse-proxy-test/ReverseProxy/default.conf nginx-base-test:/etc/nginx/conf.d/default.conf

compile it 
docker exec nginx-base-test nginx -t

reload it
docker exec nginx-base-test nginx -s reload