# 0430-docker-albums

### How to use 

> docker-end

docker-end 是使用的json-server模拟的后端服务
```bash
cd docker-end
docker build -t mikasa/albums-json .
#查看镜像
docker images
#测试运行
docker run -p 3000:80 -d mikasa/albums-json:v1
#查看运行中的容器
docker ps -a
```
浏览器访问`http://localhost:3000/albums`

> docker-front 

docker-front是有react编写的前端显示程序
- build 是react打完包后的文件夹
- dist.tar 是打包文件夹的压缩文件
```bash
cd docker-front
docker build -t mikasa/react-albums:v1
#查看镜像
docker images
#测试运行
docker run -p 8080:80 -d mikasa/react-albums:v1
#查看运行中的容器
docker ps -a
```
> 我的Docker Hub 地址

https://hub.docker.com/u/mikasa0606
