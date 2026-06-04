---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 卸载Workfront for Adobe Experience Manager增强型连接器
description: 您必须将Workfront with Adobe Experience Manager增强型连接器卸载到连接Workfront和Adobe Experience Manager Assets as a Cloud Service的最新本机集成。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
TQID: https://experienceleague.adobe.com/CeCyF8zbwp4tVcxQebq0EdaJqagDyppVuCL6ilqEvJA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 260
ht-degree: 0%

---

# 使用Adobe Experience Manager增强型连接器卸载Workfront

您必须将Workfront with Adobe Experience Manager增强型连接器卸载到连接Workfront和Adobe Experience Manager Assets as a Cloud Service的最新本机集成。

## 先决条件

* （可选）如有必要，还原对Workfront防火墙配置和AEM Dispatcher设置所做的任何更改。

## 卸载增强型连接器

1. 从Cloud Manager访问和克隆AEM as a Cloud Service存储库。

1. 在您选择的IDE中打开克隆的Git存储库。

1. 查看安装增强型连接器的分支。

1. 导航到以下路径并删除增强型连接器zip文件：

   `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. 从项目根目录的pom.xml文件中删除以下依赖项。

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
   >请确保上述代码块中引用的版本（即1.8.0）反映将从代码中卸载的版本。

1. 从名为&#x200B;**all**&#x200B;的项目子模块的pom.xml文件中删除以下依赖项。

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. 从项目名为all的子模块的pom.xml文件中删除以下嵌入内容。

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. （视情况而定）从项目根的pom.xml文件中删除存储库配置。


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. （有条件）从settings.xml（位于项目根目录的以下路径./cloudmanager/maven/settings.xml中）中删除服务器配置。

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

1. 提交更改，并将代码推送到Cloud Manager存储库

1. 运行Cloud Manager管道以在您的云服务实例上部署更改
