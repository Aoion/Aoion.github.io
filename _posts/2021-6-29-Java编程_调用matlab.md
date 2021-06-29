---
layout: post
title: 2021-06-29 Java调用matlab
date: 2021-06-29
categories: Java编程
tags: [Java编程]
description: 关于Java调用matlab

---  

## 前期准备 
	保证机器的JDK和Matlab（version -java）内置JDK版本一致 

	保证机器安装了对应版本的MCR，matlab下执行mcrinstaller可以查看MCR压缩包位置若没有则需要使用compiler.runtime.download下载（该命令下载需要科学上网），解压之后执行setup一路默认安装即可 

## 打包Matlab程序 
	matlab命令行键入deploytool，选择Library Compiler，然后按下图选择打主函数以及调用到的函数打成jar包
 
![0](https://raw.githubusercontent.com/Aoion/Aoion.github.io/master/_posts/image/2021-06-29/0.png) 

	打包完成后的for_redis_tribution_files_only下的jar包导入Java项目即可，Java部分代码网上到处都有 

## 可能报错 
	This component was created using a version of MATLAB Java Package that is not compatible with the version of MCR  

基本就是MCR的问题，按前期准备中的本机的MCR去重新安装一遍即可


	


