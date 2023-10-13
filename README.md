# xray docker build file

直接修改config文件，再编译可以省去后续挂载文件夹，方便云函数部署。

## 下载xray-xore

从https://github.com/XTLS/Xray-core/releases, 选择适当的xray内核

```bash
$ wget https://github.com/XTLS/Xray-core/releases/download/v1.8.4/Xray-linux-64.zip
$ unzip Xray-linux-64.zip
# 使用这三个文件 geoip.dat geosite.dat xray
```

## 运行构建
```bash
$ docker build -t name:version -f Dockerfile .
```
