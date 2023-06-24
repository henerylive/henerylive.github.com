---
layout: post
title: "Jenkins+Ant+Jmeterʵ�ֽӿ��Զ���"
date:   2018-10-10
tags: [Jenkins]
comments: true
author: henerylive
---

## _Jenkins+Ant+Jmeter��ӿ��Զ���_
## _Author��Henery_

Jenkins+Ant+Jmeter��Ҫ������Java�����ϣ����ж�Ӧ��JDK�汾Ҫ��

- ��װJDK
- ��װJmeter
- ��װAnt
- ��װJenkins

## 1 ��װJDK
1.1 ���ص�ַ��https://www.oracle.com/java/technologies/downloads/
1.2 �һ����ҵĵ��ԡ�����������ԡ���������߼�ϵͳ���á���������������������ҵ���ϵͳ��������������½���/���༭��
```sh
��������JAVA_HOME
����ֵ��E:\Java\jdk-17.0.7������ʵ�ʰ�װĿ¼���ã�
��������CLASSPATH
����ֵ��.;%JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\lib\tools.jar; 
��������Path
����ֵ��%JAVA_HOME%\bin;%JAVA_HOME%\jre\bin;����Path��ǰ��׷�ӣ�
```
1.3 ����JDK�Ƿ�װ�ɹ�
����cmd����������java -version����java��javac��
```sh
java -version
```
���óɹ�����ʾjava�汾��Ϣ��
java version "17.0.7" 2023-04-18 LTS
Java(TM) SE Runtime Environment (build 17.0.7+8-LTS-224)
Java HotSpot(TM) 64-Bit Server VM (build 17.0.7+8-LTS-224, mixed mode, sharing)

## 2 ��װJmeter
2.1 ���ص�ַ��https://jmeter.apache.org/download_jmeter.cgi
2.2 ��ѹJmeter�ļ���˫��Jmeter��binĿ¼�µ�jmeter.bat�����п��ӻ����棬������ʧ�ܴ������JDK�汾����Ӧ����������ڵ���ʾ�Ҷ�Ӧ�İ汾����ѹ���ٴ����м��ɡ�

## 3 ��װAnt
3.1 ���ص�ַ��https://ant.apache.org/bindownload.cgi
3.2 ��ѹAnt�ļ�
3.3 �һ����ҵĵ��ԡ�����������ԡ���������߼�ϵͳ���á���������������������ҵ���ϵͳ��������������½���/���༭��
```sh
��������ANT_HOME
����ֵ��E:\apache-ant-1.9.16������ʵ�ʰ�װĿ¼���ã�
��������Path
����ֵ��%ANT_HOME%\bin;����Path��ǰ��׷�ӣ�
```
3.4 ����Ant�Ƿ�װ�ɹ�
����cmd����������ant -version��
```sh
ant -version
```
���óɹ�����ʾant�汾��Ϣ��
Apache Ant(TM) version 1.9.16 compiled on July 10 2021

## 4 ��װJenkins
4.1 ���ص�ַ��https://www.jenkins.io/zh/download/
4.2 ��װ�����뱣����C:\Users\guohl\.jenkins\secrets\initialAdminPassword�ļ��У�·������װ�����
