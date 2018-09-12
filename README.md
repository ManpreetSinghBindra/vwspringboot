docker pull mongo

docker run -P -d --name mongodb mongo

docker build -t springrestmongodbdemo .

docker images

docker run -p 8888:8081 -P -d --name employee --link mongodb springrestmongodbdemo
