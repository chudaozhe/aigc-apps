# Magika
`Magika` 是一种使用深度学习检测常见文件内容类型的工具。

构建镜像
```
docker build -t chudaozhe/magika:0.5.1 .
```

使用
```
#检测当前目录的文件类型
docker run -it --rm -v .:/magika chudaozhe/magika:0.5.1 -r /magika --json
#帮助
docker run -it --rm chudaozhe/magika:0.5.1 -h
#版本
docker run -it --rm chudaozhe/magika:0.5.1 --version
```

## 参考
https://google.github.io/magika/