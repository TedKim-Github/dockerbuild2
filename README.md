# Building & Running

Copy the sources to your docker host and build the container, and to run.
```
	docker build --rm -t abbasidoc/ubuntu-nginx .
	docker run -it --name cn1 -e USER=abbasidoc -e PASSWD=abbasidoc -v c:\\Users\\user\\df:/var/www/html -p 80:80 abbasidoc/ubuntu-nginx
```
To test, ("nowage" is username. )
```
  open 127.0.0.1
	su - abbasidoc
```
To Rollback
```
    docker rm cn1 -f
    docker rmi abbasidoc/ubuntu-nginx
```
