---
layout: post
title: Cubieboard开发版测试
date: 2013-03-21 13:11:26
category: cubieboard
published: true
tags: Cubieboard 开发板
---

安装VNC
	sudo apt-get install tightvncserver

修改xstartup文件
	~/.vnc/xstartup
	输入以下内容
		#!/bin/sh
		startlubuntu &

启动VNC
	tightvncserver -geometry 800x600 :1 
	
如果首次启动，输入vncpasswd设置密码

PS：可以将启动命令加入/etc/rc.local开机启动。


关闭VNC
	tightvncserver -kill :1


安装完后可以直接这Windows下连接VNC（通过VNC Viewer）
	