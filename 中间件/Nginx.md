# Nginx

## 基础介绍

### nginx
```yaml
nginx:
    -s:
        quit:
        reload:
        reopen:
        stop:
    -t: 检查配置文件语法
    -V: 详细信息
```
#### nginx.conf
```yaml
nginx.conf:
    error_log: 错误日志路径
    events: 网络连接配置
        worker_connections:
    http: http配置
        default_type:
        include: 引入其他配置
        keepalive_timeout:
        log_format: 日志格式
        sendfile: 
        server: http服务配置（可配置多个）
            error_page: 错误页面
            listen:
            location: 目录映射
                index: 首页
                proxy_pass: 代理
                root: 根目录
                

            server_name: 域名
        ssl_certificate: 证书pem
        ssl_certificate_key: 密钥key
    worker_processes: 工作进程数
    upstream:
        ip_hash:
        server:
            weight:
            
```

master与worker进程



## 核心内容


