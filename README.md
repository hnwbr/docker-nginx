# docker-nginx

sudo docker network create nginx && \
sudo docker volume create var-lib-nginx && \
sudo docker volume create etc-nginx-templates

```bash

docker compose run --rm certbot certonly --webroot --webroot-path /var/www/certbot/ --dry-run -d example.org

sudo crontab -e

0 */12 * * * docker-compose -f /path/to/docker-compose.yaml run certbot renew --quiet && docker-compose -f /path/to/docker-compose.yaml kill -s SIGHUP nginx

docker-compose run certbot certonly --dns-dnsprovider --dns-dnsprovider-credentials /path/to/credentials.ini -d example.com

```

https://hub.docker.com/r/certbot/dns-cloudflare
https://eff-certbot.readthedocs.io/en/stable/install.html#running-with-docker

https://github.com/GoogleCloudPlatform/community/blob/master/archived/nginx-reverse-proxy-docker.md
https://github.com/eugene-khyst/letsencrypt-docker-compose
https://github.com/bringnow/docker-nginx-letsencrypt

https://mindsers.blog/post/https-using-nginx-certbot-docker/
https://www.digitalocean.com/community/tutorials/how-to-secure-a-containerized-node-js-application-with-nginx-let-s-encrypt-and-docker-compose
https://stackify.com/how-to-configure-https-for-an-nginx-docker-container/
https://www.programonaut.com/setup-ssl-with-docker-nginx-and-lets-encrypt/
https://mpolinowski.github.io/docs/DevOps/NGINX/2020-08-28--nginx-docker-certbot/2020-08-27/
https://medium.com/rahasak/setup-lets-encrypt-certificate-with-nginx-certbot-and-docker-b13010a12994
https://gilyes.com/docker-nginx-letsencrypt/
https://www.freecodecamp.org/news/docker-nginx-letsencrypt-easy-secure-reverse-proxy-40165ba3aee2/
