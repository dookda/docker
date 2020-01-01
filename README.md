# docker
check version
```
docker version
```
pull image
```
docker pull IMAGE
```
list docker image
```
docker images
```
docker run
```
docker run [options] IMAGE
```
```
docker run --name [ระบุชื่อ] -d -p 8080:80 [ชื่อ image / image id ที่ต้องการ]
```

docker exec เข้าไปใช้ linux cli ใน image
```
docker exec [options] CONTAINER COMMAND
  -d, --detach        # run in background
  -i, --interactive   # stdin
  -t, --tty           # interactive
```

```
docker exec -it [ชื่อ image] bash
```

ออกจาก containner
```
exit
```
