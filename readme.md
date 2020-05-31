# Dockerfile

树莓派 4 上运行的 Docker

## 准备

在启动之前，先创建共享 network

```sh
docker network create local_work
```

## 服务

- [x] baidu.local.cc (5299)
- [x] file.local.cc (4399)
- [x] npm.local.cc (4873)
- [x] swirl.local.cc (8001)
- [x] netdata.local.cc (19999)
- [ ] git.local.cc ()