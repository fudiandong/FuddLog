# 学习日志管理系统

## 项目简介

基于JeeSite框架开发一套能把日常遇到的问题及学到的知识记录起来的管理系统----FuddLog

1、修改生成代码路径，报 页面不存在
    解决方法： spring-context.xml 在 24,31,40行添加 生成路径 如 新生成代码 路径为 com.fudd.record ，可在  xml中修改为  <property name="basePackage" value="com.thinkgem.jeesite;com.fudd"/>
    或者 将spring的扫描路径改为 根目录 com 等
    spring-mvc.xml  第14行  <context:component-scan base-package="com.thinkgem.jeesite;com.cabinetms" use-default-filters="false"><!-- base-package 如果多个，用“,”分隔 -->
