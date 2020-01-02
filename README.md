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

check doeker run
```
docker ps
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

mouth drive
```
docker run --name mysql-db -v D:/dockershare/mysql:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=111111 -d mysql
```

mouth wordpress with multiline
```
docker run -d --name docker-press -p 80:80 --link mysql-db:mysql `
-v Q:/sharevolume/wordpress:/var/www/html `
-e WORDPRESS_DB_HOST=mysql `
-e WORDPRESS_DB_USER=root `
-e WORDPRESS_DB_PASSWORD=111111 `
 wordpress 
 ```
