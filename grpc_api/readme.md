# grpc 接口定义（protobuf 结构体）

# gRPC 接口定义（protobuf 结构体）

注：

1. proto 结构体文件按照包名分类，同级放在同一目录中

实际应用中, 后者速度相对更快. 但是需要设置如 gRPC 超时时间等参数时只能使用前者.

3. 以下文件全部来自 apk 的逆向工程，如有疏漏请包涵

## grpc 主机

B 站客户端的 grpc 接口主机为以下服务器

参考 [gRPC Go 官方文档](https://github.com/grpc/grpc-go/blob/master/Documentation/grpc-metadata.md) 对 `Metadata` 的说明.

## grpc 鉴权

需要在请求 http 头部中添加`access_key`，如下

需要的 `Metadata` 包括(但不限于):

## grpc 头部

-   [bilibili.metadata](bilibili/metadata)：客户端环境参数
-   [bilibili.rpc](bilibili/rpc/status.proto)：响应错误信息

## 接口请求定义

_稍后补充_
