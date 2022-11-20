# 搭建go protoc编译环境
1. 本容器集成了 grpc, grpc-gateway, openapiv2, go 插件
2. 使用buf代替protoc

# 文档
- [buf文档](https://docs.buf.build/how-to/replace-protoc-with-buf)
- [gateway文档](https://github.com/grpc-ecosystem/grpc-gateway)
- [validate文档](https://github.com/bufbuild/protoc-gen-validate)
- [golang protobuf](https://github.com/golang/protobuf)

# 安装说明
1. 从github上下载buf应用文件来代替线上安装， 若需要线上安装，请使用下方连接， 此处使用的buf版本为1.9.0版本
```shell
curl -sSL "https://github.com/bufbuild/buf/releases/download/v1.9.0/buf-$(uname -s)-$(uname -m)"
```

# docker仓库地址
https://hub.docker.com/repository/docker/zxc7310/buf

# 使用方法
```shell
docker run --rm -v "$(pwd):/workspace" --workdir /workspace zxc7310/buf:v1.0 lint
```