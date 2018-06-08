# dockerfile
jenkins
docker run -it --rm -p 8888:8080 tomcat:8.0 -- tomcat image 
docker run --name some-mysql -e MYSQL_ROOT_PASSWORD=my-secret-pw -d mysql:8.0

docker run --name tomcat:8.0 --link some-mysql:mysql -d some-mysql
