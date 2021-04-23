# 预编译的DLV
方便调试golang程序。

# Linux快速安装

`curl -L https://raw.fastgit.org/snail007/dlv/main/go1.13-1.15/linux/dlv;chmod +x dlv;mv dlv /usr/bin/`

# Macos快速安装

`curl -L https://raw.fastgit.org/snail007/dlv/main/go1.13-1.15/linux/dlv;chmod +x dlv;mv dlv /usr/local/bin/`

# 示例

## 程序不带参数

```shell
dlv --headless=true --check-go-version=false --accept-multiclient --api-version=2 --listen=:62231 exec ./foo
```

## 程序带参数

```shell
dlv --headless=true --check-go-version=false --accept-multiclient --api-version=2 --listen=:62231 exec ./foo -- --foo
```
