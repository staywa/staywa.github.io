---
title: Maven项目管理工具安装配置
---
https://blog.csdn.net/weixin_38568503/article/details/121045947

#### 阿里云镜像库：
 <mirror>
    <id>alimaven</id>
    <mirrorOf>central</mirrorOf>
    <name>aliyun maven</name>
    <url>http://maven.aliyun.com/nexus/content/repositories/central/</url>
 </mirror>`

#### 修改java的版本
 <!-- java版本 --> 
 `<profile>`
      <id>jdk-1.8</id>
      <activation>
        <activeByDefault>true</activeByDefault>
        <jdk>1.8</jdk>
      </activation>
      <properties>
        <maven.compiler.source>1.8</maven.compiler.source>
        <maven.compiler.target>1.8</maven.compiler.target>
        <maven.compiler.compilerVersion>1.8</maven.compiler.compilerVersion>
      </properties>
 </profile>