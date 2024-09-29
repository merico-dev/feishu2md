编译本项目的 `CLI` 版本：

```bash
go build -ldflags="-s -w -X main.version=`git rev-parse --short HEAD`@amd64-linux" -o ./feishu2md cmd/*.go
```

压缩编译好的二进制可执行文件：

```bash
upx -9 ./feishu2md
```
