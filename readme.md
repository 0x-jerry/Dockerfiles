# Dockerfile

利用 Hosts 和 Nginx 来隐藏端口和 IP 地址

在启动之前，先创建共享 network

```sh
docker network create local_work
```