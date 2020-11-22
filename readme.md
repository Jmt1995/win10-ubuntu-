# win10远程连接原生的ubuntu桌面

## 引言

远程连接Linux服务器的方式多种多样，有：

1. SSH连接 命令行样式

2. 可视化连接 桌面风格

今天我们主要介绍的是可视化连接, 故名思意即远程桌面控制，常见的可视化连接有两种
**xrdp**和 **vnc**，在这里我们对比一下这两者的区别
## xrdp 与 vnc 区别
![区别](./images/1difference.png)

## 通过XDRP实现Windows远程连接
**不推荐这种方法**，该方法是通过第三方桌面系统实现远程访问
 1. #安装xrdp 
> sudo apt-get install xrdp 
 2. #安装vnc4server 
> apt-get install vnc4server tightvncserver
 3. #安装xubuntu-desktop 
> sudo apt-get install xubuntu-desktop 
 4. #向xsession中写入xfce4-session 
> echo “xfce4-session” >~/.xsession 
 5. #开启xrdp服务 
> sudo service xrdp restart
下面讲解的是如何直接访问原生系统
## 通过VNC实现Windows远程连接


## 如若本文图片未显示

请点击链接[解决GitHub中图片不显示](https://github.com/Jmt1995/PictureError)


git remote add origin git@github.com:Jmt1995/win10-ubuntu-.git