# phddns, archlinux 安装文件

花生壳内网穿透客户端 [phddns](https://hsk.oray.com/download/)，官网只有 deb 和 rpm 安装包。

拆开 deb 安装文件(version 3.0)，将必有的 二进制文件以及脚本提取出来，少量修改，使用 systemd 实现开机启动(systemctl status 不正常)。

按照路径放置文件，添加必要的权限。

```sh
sudo systemctl daemon-reload

sudo systemctl enable phddns
```


