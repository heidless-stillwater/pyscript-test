
# dockerfile 
```
FROM nginx:alpine
COPY . /usr/share/nginx/html
```

# build
```
docker build -t html-server-image:v1 .

docker images
```
# run
```
docker run -d -p 80:80 html-server-image:v1
```

# test
```
curl localhost:80

http://localhost:80
```