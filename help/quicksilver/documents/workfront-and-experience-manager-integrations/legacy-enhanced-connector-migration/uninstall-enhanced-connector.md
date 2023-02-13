---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 卸载Workfront for Adobe Experience Manager增强连接器
description: 您必须卸载带有Adobe Experience Manager的Workfront增强连接器，以连接到连接Workfront和Adobe Experience Manager Assets的最新本机集成as a Cloud Service。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 使用Adobe Experience Manager增强连接器卸载Workfront

您必须卸载带有Adobe Experience Manager的Workfront增强连接器，以连接到连接Workfront和Adobe Experience Manager Assets的最新本机集成as a Cloud Service。

## 先决条件

* （可选）根据需要，还原对Workfront防火墙配置和AEM调度程序设置所做的任何更改。

## 卸载增强的连接器

1. 从Cloud Manager访问和克隆AEMas a Cloud Service存储库。

1. 在选择的IDE中打开克隆的git存储库。

1. 签出安装增强连接器的分支。

1. 导航到以下路径并删除增强的连接器zip文件：

   `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. 从项目根的pom.xml文件中删除以下依赖项。

   ```
   <!-- Workfront Tools -->
    <dependency>
        <groupId>digital.hoodoo</groupId>
        <artifactId>workfront-tools.ui.apps</artifactId>
        <type>zip</type>
        <version>1.8.0</version>
        <scope>system</scope>
        <systemPath>${project.basedir}/ui.apps/src/main/resources/workfront-tools.ui.apps.zip</systemPath>
    </dependency>
   ```

   >[!NOTE]
   >
   >请确保上述代码块（即1.8.0）中引用的版本反映了从代码中卸载的版本。

1. 从项目子模块的pom.xml文件中删除以下依赖项，该文件名为 **全部**.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```
1. 从项目子模块名为all的pom.xml文件中删除嵌入的以下内容。

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. （视情况而定）从项目根目录的pom.xml文件中删除存储库配置。


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. （视情况而定）从以下路径中存在的settings.xml中删除服务器配置。/cloudmanager/maven/settings.xml在项目根目录中。

   ```
           <server>
           <id>hoodoo-maven</id>
           <configuration>
               <httpHeaders>
                   <property>
                       <name>Deploy-Token</name>
                       <value>*********************</value>
                   </property>
               </httpHeaders>
           </configuration>
       </server>
   ```

1. 提交更改，然后将代码推送到Cloud Manager存储库

1. 运行Cloud Manager管道以在您的Cloud Services实例上部署更改
