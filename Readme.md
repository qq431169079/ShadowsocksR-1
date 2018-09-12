# ShadowsockR Server Installation
This is the installation shell script of ShadowsocksR for Linux server, which are VPS that running by host suppliers, or physical server by someone's own, etc.
The source codes of this shell script were written by breakwa11 and updated by teddysun.
## 
## ShadowsocksR一键安装脚本
本脚本适用环境：
系统支持：CentOS，Debian，Ubuntu
内存要求：≥128M
## 关于本脚本：
一键安装 ShadowsocksR 服务端。请下载与之配套的客户端程序来连接。
## 
（以下客户端只有 Windows 客户端和 Python 版客户端可以使用 SSR 新特性，其他原版客户端只能以兼容的方式连接 SSR 服务器）
## 使用方法：
使用root用户登录，运行以下命令：
## 
wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh
## 
chmod +x shadowsocksR.sh
## 
./shadowsocksR.sh 2>&1 | tee shadowsocksR.log
## 卸载方法：
使用 root 用户登录，运行以下命令：
./shadowsocksR.sh uninstall
## 安装完成后即已后台启动 ShadowsocksR ，运行：
/etc/init.d/shadowsocks status
可以查看 ShadowsocksR 进程是否已经启动。
本脚本安装完成后，已将 ShadowsocksR 自动加入开机自启动。
## 使用命令：
启动：/etc/init.d/shadowsocks start
停止：/etc/init.d/shadowsocks stop
重启：/etc/init.d/shadowsocks restart
状态：/etc/init.d/shadowsocks status
## 
配置文件路径：/etc/shadowsocks.json
日志文件路径：/var/log/shadowsocks.log
代码安装目录：/usr/local/shadowsocks
## 如果你想修改配置文件，请参考：
https://github.com/shadowsocksr-backup/shadowsocks-rss/wiki/Server-Setup
https://github.com/shadowsocksr-backup/shadowsocks-rss/blob/master/ssr.md
https://github.com/shadowsocksr-backup/shadowsocks-rss/wiki/config.json
## 参考链接：
https://github.com/shadowsocksr-backup/shadowsocksr

