---
layout: post
title: El未生效
category: bug日常
tags: el
key: el
description: web项目中el不生效缘由
---

### el表达式不生效，显示 ${xxx}的原因

	<web-app xmlns="http://java.sun.com/xml/ns/javaee"
    	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    	xsi:schemaLocation="http://java.sun.com/xml/ns/javaee
    	http://java.sun.com/xml/ns/javaee/web-app_2_5.xsd" 
		version="2.5">

> 2.4版本默认支持el表达式，如果使用2.5版本，默认el表达式是关闭的

2.5版本应在jsp页面头部添加 **<%@ page isELIgnored="false"%>**

转自：[http://kim.iteye.com/blog/202090](http://kim.iteye.com/blog/202090)