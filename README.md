# shell-clash
Installation Guide of ShellClash on Xiaomi Route 3 PRO

官方下载：https://github.com/juewuy/ShellClash/raw/master/bin/ShellClash.tar.gz

参考文档：
https://www.homaton.com/router/xiaomi-ax3600.html

## 安装开发版固件 + 启用SSH
http://www1.miwifi.com/miwifi_download.html
https://d.miwifi.com/rom/ssh

## 安装设置Clash

登录后创建 /etc/clash 目录

复制ShellClash.tar.gz到/etc/clash

解压缩tar xzvf ShellClash.tar.gz

运行./clash.sh

按照向导进行配置，然后执行以下步骤

6 导入配置文件

2 导入Clash配置文件链接：输入Clash订阅链接

按提示启动Clash（会自动运行）。

## 自动切换代理

在clash安装目录下找到config.yaml，download到本地，编辑proxy group type（从select改为url-test, 增加interval: 300）:

```
proxy-groups:
  -
    name: '🚀 节点选择'
    type: url-test
    interval: 300
```
