---
layout: post
title: "Jenkins+Ant+Jmeter实现接口自动化"
date:   2018-10-10
tags: [Jenkins]
comments: true
author: henerylive
---

今天记录的是Jenkins+Ant+Jmeter的搭建

<!-- more -->

## _Jenkins+Ant+Jmeter搭建接口自动化_
## _Author：Henery_

Jenkins+Ant+Jmeter需要运行在Java环境上，且有对应的JDK版本要求。

- 安装JDK
- 安装Jmeter
- 安装Ant
- 安装Jenkins

## 1 安装JDK
1.1 下载地址：https://www.oracle.com/java/technologies/downloads/
1.2 右击“我的电脑”，点击“属性”，点击“高级系统设置”，点击“环境变量”，找到“系统变量”，点击“新建”/“编辑”
```yml
变量名：JAVA_HOME
变量值：E:\Java\jdk-17.0.7（根据实际安装目录配置）
变量名：CLASSPATH
变量值：.;%JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\lib\tools.jar; 
变量名：Path
变量值：%JAVA_HOME%\bin;%JAVA_HOME%\jre\bin;（在Path最前边追加）
```
1.3 测试JDK是否安装成功
运行cmd，键入命令java -version或者java或javac：
```yml
java -version
```
配置成功，显示java版本信息：
java version "17.0.7" 2023-04-18 LTS
Java(TM) SE Runtime Environment (build 17.0.7+8-LTS-224)
Java HotSpot(TM) 64-Bit Server VM (build 17.0.7+8-LTS-224, mixed mode, sharing)

## 2 安装Jmeter
2.1 下载地址：https://jmeter.apache.org/download_jmeter.cgi
2.2 解压Jmeter文件，双击Jmeter的bin目录下的jmeter.bat，运行可视化界面，，运行失败大概率是JDK版本不对应，根据命令窗口的提示找对应的版本，解压后再次运行即可。

## 3 安装Ant
3.1 下载地址：https://ant.apache.org/bindownload.cgi
3.2 解压Ant文件
3.3 右击“我的电脑”，点击“属性”，点击“高级系统设置”，点击“环境变量”，找到“系统变量”，点击“新建”/“编辑”
```yml
变量名：ANT_HOME
变量值：E:\apache-ant-1.9.16（根据实际安装目录配置）
变量名：Path
变量值：%ANT_HOME%\bin;（在Path最前边追加）
```
3.4 测试Ant是否安装成功
运行cmd，键入命令ant -version：
```yml
ant -version
```
配置成功，显示ant版本信息：
Apache Ant(TM) version 1.9.16 compiled on July 10 2021

## 4 安装Jenkins
4.1 下载地址：https://www.jenkins.io/zh/download/
4.2 安装后，密码保存在C:\Users\guohl\.jenkins\secrets\initialAdminPassword文件中（路径看安装情况）
