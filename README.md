# docker-nginx

sudo docker network create net_nginx && \
sudo docker volume create var-lib-nginx && \
sudo docker volume create etc-nginx-templates

<!-- sudo crontab -e -->
<!-- 0 */12 * * * docker-compose -f /path/to/docker-compose.yaml run certbot renew --quiet && docker-compose -f /path/to/docker-compose.yaml kill -s SIGHUP nginx -->
<!-- docker-compose run certbot certonly --dns-dnsprovider --dns-dnsprovider-credentials /path/to/credentials.ini -d example.com -->

https://hub.docker.com/r/certbot/dns-cloudflare

https://eff-certbot.readthedocs.io/en/stable/install.html#running-with-docker

https://mindsers.blog/post/https-using-nginx-certbot-docker/

https://www.digitalocean.com/community/tutorials/how-to-run-nginx-in-a-docker-container-on-ubuntu-22-04

https://www.digitalocean.com/community/tutorials/how-to-secure-a-containerized-node-js-application-with-nginx-let-s-encrypt-and-docker-compose

https://stackify.com/how-to-configure-https-for-an-nginx-docker-container/

https://www.programonaut.com/setup-ssl-with-docker-nginx-and-lets-encrypt/

https://github.com/eugene-khyst/letsencrypt-docker-compose

https://mpolinowski.github.io/docs/DevOps/NGINX/2020-08-28--nginx-docker-certbot/2020-08-27/
https://medium.com/rahasak/setup-lets-encrypt-certificate-with-nginx-certbot-and-docker-b13010a12994
https://gilyes.com/docker-nginx-letsencrypt/
https://www.freecodecamp.org/news/docker-nginx-letsencrypt-easy-secure-reverse-proxy-40165ba3aee2/
