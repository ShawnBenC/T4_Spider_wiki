## 创建镜像

`docker image build -t tv:latest .`

## 运行容器

`docker run --name TV --net="host" -v /opt/TV（源码所在目录）:/TV tv:latest gunicorn -w 4 -b 0.0.0.0:8080 app:app`

## 脚本安装、更新

## 注意
- 需要提前安装unzip：
```
openwrt：opkg update && opkg install unzip
ubuntu、debian：apt-get update && apt-get install unzip
其他系统自行百度
```