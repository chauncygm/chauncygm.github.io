---
layout: post
title: Spring Boot报错
category: bug日常
tags: springboot
key: springboot
description: spring boot 项目错误
---

##spring boot

报错如下：

> ** WARNING ** : Your ApplicationContext is unlikely to start due to a @ComponentScan of the default package.
> 
> 即：ApplicationContext不能从一个组件的默认包启动

解决办法：

* 建一个新包，将applicationContext放在其中或放入其他包下