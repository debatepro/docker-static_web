# docker-static_web

# GIT

Update from Github
```
git pull
```

Update from local machine
```
git commit -m "<comment>"
git add -A
git push origin master
```

# Docker
One liner to stop / remove all of Docker containers:
```
sudo docker stop $(sudo docker ps -a -q)
sudo docker rm $(sudo docker ps -a -q)
```

Running containers:
```
# -P use all ports specified in the Dockerfile
sudo docker run -d -P --name <name> <db8pro/name>

# Bind to specific port
sudo docker run -d -p 8080:80 --name <name> <db8pro/name>

# Bind to random port 
sudo docker run -d -p 127.0.0.1::80 --name <name> <db8pro/name>

# Bind to specific interface  
sudo docker run -d -p 127.0.0.1:80:80 --name <name> <db8pro/name>

# Specify /UDP

```
