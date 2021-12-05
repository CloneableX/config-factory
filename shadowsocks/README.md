## 安装 shadowsocks

apt install shadowsocks-libev
apt install proxychains

## 配置 shadowsocks

配置 /etc/shadowsocks-libev/config.json，参考 [config.json](./config.json)

设置 shadowsocks-libev 开机启动

sudo systemctl start shadowsocks-libev-local@config
sudo systemctl enable shadowsocks-libev-local@config

查看任务状态

sudo systemctl status shadowsocks-libev-local@config

## 配置 proxychains

将 /etc/proxychains.conf 文件最后一行设置为 `socks5 127.0.0.1 1080`，具体参考 [proxychains.conf](./proxychains.conf)

在终端中需要代理时在开始增加 proxychains 命令即可，如 `proxychains curl ~`

## chrome 安装插件

为 chrome 安装 SwitchyOmega 插件，下载地址 https://github.com/FelisCatus/SwitchyOmega/releases

SwitchyOmega 自动摘取 pac 规则，在 Rule List URL 填写拉取地址

```
https://raw.githubusercontent.com/gfwlist/gfwlist/master/gfwlist.txt
```
