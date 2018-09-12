docker pull mongo

docker run -P -d --name mongodb mongo

docker build -t springrestmongodbdemo .

docker images

docker run -p 8888:8081 -P -d --name employee --link mongodb springrestmongodbdemo

-----------------------------------------------------------------

cf login -a api.run.pivotal.io

cf push springcfdemo  -p target/springcfdemo-0.0.1-SNAPSHOT.jar

cf logout

