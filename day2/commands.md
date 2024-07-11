```
docker container run -it ubuntu bash
apt update
apt install python3
python3 -V
apt install nodejs
nodejs -v
exit
docker container ls -a
# COPY container ID and paste below
docker commit container ID custom-image
docker image ls

git clone https://github.com/arjunachari12/docker-demo-with-simple-python-app.git 
#Docker build command
docker build -t my-python-app:1.0.0 .

#Create docker registry in docker hub called as my-python-app, copy the registry name
docker tag my-python-app:1.0.0 arjunachari12/my-python-app:1.0.0
docker login
Docker push arjunachari12/my-python-app:1.0.0

###########################
Network Commands

docker network ls
docker network inspect bridge
docker network ls
docker network create my_app_net
docker network ls
docker network create --help
docker container run -d --name new_nginx --network my_app_net nginx
docker network inspect my_app_net

==============================
docker container run -d --name mysql -e MYSQL_ALLOW_EMPTY_PASSWORD=True mysql
docker container inspect mysql
docker volume ls
docker volume inspect TAB COMPLETION
docker volume create mysql-db
docker container run -d --name mysql -e MYSQL_ALLOW_EMPTY_PASSWORD=True -v mysql-db:/var/lib/mysql mysql

Volume commands
mkdir html
#add index.html page under html folder
#add some text as “Welcome to Bind mount”
cd html
docker container run -d --name nginx -p 80:80 -v $(pwd):/usr/share/nginx/html nginx



```
