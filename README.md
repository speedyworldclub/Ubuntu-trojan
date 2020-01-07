# trojan-wiz
一键安装trojan-gfw
## 安装前必须打开服务器的80和443端口
---
# 安装命令：
> wget -N --no-check-certificate https://raw.githubusercontent.com/mark-hans/trojan-wiz/master/ins.sh && chmod +x ins.sh && sudo bash  ins.sh
---
支持的系统：
- ubuntu 16.04+
- debian 9(理论上应该支持debian 8)
- centos 7+


# 给作者一些改进和升级这个脚本的动力：
![Image text](https://raw.githubusercontent.com/mark-hans/trojan-wiz/master/images/1.jpg)
![Image text](https://raw.githubusercontent.com/mark-hans/trojan-wiz/master/images/2.jpg)
![Image text](https://raw.githubusercontent.com/mark-hans/trojan-wiz/master/images/3.jpg)





2.一键安装trojan，并自动进行配置
3,054 views

Mark Logs【马克·罗格斯】
Published on Feb 11, 2019
购买VPS服务器请戳:
搬瓦工：http://bit.ly/2FHfp4m
数字海洋：http://bit.ly/2uCIffL

一键安装trojan，并自动配置
---------------------------------------------
google云服务器设置，开启root登录

vi /etc/ssh/sshd_config

PermitRootLogin yes //默认为no，需要开启root用户访问改为yes



PasswordAuthentication yes //默认为no，改为yes开启密码登陆
systemctl restart sshd
---------------------
安装wget:
Centos : sudo yum install wget
ubuntu/Debian: sudo apt install wget 
------------------------
运行trojan一键安装命令：
wget -N --no-check-certificate https://raw.githubusercontent.com/mar... && chmod +x ins.sh && sudo bash ins.sh
安装完成启动：服务端
输入：systemctl start trojan-gfw
-------------------
项目地址：
https://github.com/mark-hans/trojan-wiz
