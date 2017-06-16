# 高性能计算平台搭建日志 #


### 安装环境 ###
- vmware 12.5.1
- centOS 7

## 安装过程 ##

### 首先创建一个名为 ma 的虚拟机 ###
- <h4> <a href="http://blog.sina.com.cn/s/blog_712a465c0102v4h5.html"> 安装教程 </a> </h4>

### 创建一个名为 cn 的虚拟机  ###

- <h4> <a href = "https://jingyan.baidu.com/article/6b97984d9798f11ca2b0bfcd.html">克隆虚拟机ma </a> <h4>

nmcli c modify "有线连接 1" ipv4.addresses 192.168.91.10/24

nmcli c modify "有线连接 1" ipv4.gateway 192.168.91.1

nmcli c modify "有线连接 1" ipv4.dns 192.168.91.1 

nmcli c modify "有线连接 1" ipv4.method manual 

nmcli c down "有线连接 1"; nmcli c up "有线连接 1"

nmcli d show "有线连接 1"
