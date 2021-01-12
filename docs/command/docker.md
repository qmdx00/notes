### Docker 相关命令

阿里云安装docker脚本
```bash
curl -fsSL https://get.docker.com | bash -s docker --mirror Aliyun
```

docker 启动 Mysql
```
docker run -d --name mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=123 mysql:latest
```

docker 启动 Redis
```
docker run -d --name redis -p 6379:6379 redis:latest --requirepass "123"
```