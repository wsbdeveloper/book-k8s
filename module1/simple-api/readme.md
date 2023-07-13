## Create image from DockerHub

Create image for send application in container.

```bash
docker build -t simple-api-nodejs .
```

Running the image.

```bash
docker run -e PORT=8081 -p 2345:8080 simple-api-nodejs
```

Prepare image for send the docker hub.

```bash
docker tag simple-api-nodejs wellingtondocker/simple-api-nodejs
```
