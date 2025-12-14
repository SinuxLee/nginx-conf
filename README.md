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

### WebDAV in NGINX
nginx 自带一个 dav 模块，可以用于网页浏览。但不支持 dav client 的协议访问。https://github.com/arut/nginx-dav-ext-module.git 是一个dav扩展模块，需要重新编译nginx。
