## ShadowsockR Server Installation
This is the installation shell script of ShadowsocksR for Linux server, which are VPS that running by host suppliers, or physical server by someone's own, etc. <br>
The source codes of this shell script were written by breakwa11 and updated by teddysun.

### ShadowsocksR一键安装脚本
本脚本适用环境：<br>
系统支持：CentOS，Debian，Ubuntu <br>
内存要求：≥128M

### 关于本脚本：
一键安装 ShadowsocksR 服务端。请下载与之配套的客户端程序来连接。<br>
（以下客户端只有 Windows 客户端和 Python 版客户端可以使用 SSR 新特性，其他原版客户端只能以兼容的方式连接 SSR 服务器）

### 使用方法：
使用root用户登录，运行以下命令：(本脚本安装完成后，已将 ShadowsocksR 自动加入开机自启动。)
<br>
>>wget --no-check-certificate https://github.com/uwtom/SSR_Server_Install/raw/master/shadowsocksR.sh <br>
>>chmod +x shadowsocksR.sh <br>
>>./shadowsocksR.sh 2>&1 | tee shadowsocksR.log

### 卸载方法：
使用 root 用户登录，运行以下命令：<br>
./shadowsocksR.sh uninstall

### 安装完成后即已后台启动 ShadowsocksR ，运行：
/etc/init.d/shadowsocks status <br>
可以查看 ShadowsocksR 进程是否已经启动。

### 使用命令：
启动：/etc/init.d/shadowsocks start <br>
停止：/etc/init.d/shadowsocks stop <br>
重启：/etc/init.d/shadowsocks restart <br>
状态：/etc/init.d/shadowsocks status <br><br>
配置文件路径：/etc/shadowsocks.json <br>
日志文件路径：/var/log/shadowsocks.log <br>
代码安装目录：/usr/local/shadowsocks

### 参考链接：
https://github.com/uwtom/SSR_Server_Install/wiki/ShadowsocksR-Server-Setup
