# docker-run-to-compose-demo

Demo of converting a Docker run command to Docker compose.

Before:

```bash
docker run -dit --name docker-run-to-compose-demo -p 8080:80 --mount type=bind,src="${PWD}/src",dst=/usr/local/apache2/htdocs/ httpd:2.4
```

After:

```bash
docker-compose up -d
```
