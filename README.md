# docker-static_web

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


One liner to stop / remove all of Docker containers:
```
sudo docker stop $(sudo docker ps -a -q)
sudo docker rm $(sudo docker ps -a -q)
```
