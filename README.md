# Nginx 配置文件

### 目录
- cert 存放证书
- www 存放网页等静态资源
- logs 存放日志及pid文件
- conf 一些通用配置
- conf.d 存储虚拟主机的配置

### 安全

### 性能

### 运行
1. Docker 方式使用
```
docker run -d \
--name nginx \
-p 8080:80  \
-v $PWD:/etc/nginx \
--restart=always  \
nginx
```
