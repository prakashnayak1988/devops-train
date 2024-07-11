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

#Docker build command
docker build -t my-python-app:1.0.0 .

```
