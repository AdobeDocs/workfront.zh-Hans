---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 卸载旧版连接器
description: 文本
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# 使用Adobe Experience Manager旧版连接器卸载Workfront

您必须将Workfront与Adobe Experience Manager旧版连接器卸载到连接Workfront和Adobe Experience Manager Assetsas a Cloud Service的最新本机集成。

## 取消订阅Workfront

1. 打开AdobeExperience Manger。
1. 在Experience Manager中，转到&#x200B;**Cloud Service** > **工具** > **Workfront集成配置**。
1. 选择您的配置（默认为global-workfront），然后单击&#x200B;**属性**。
   ![取消订阅workfront](assets/unsubscribe-from-workfront.png)
1. 禁用文档、注释和元数据同步。 该标签天应为“禁用”。
这将删除Workfront中的订阅，并允许用户使用Day CQ Link Externalizer中定义的相同URL创建新订阅。

## 删除Workfront集成配置

现在，在删除订阅后，可以安全地删除Workfront集成配置。

1. 打开配置，然后选择&#x200B;**删除**。
   ![删除配置](assets/delete-wf-configuration.png)

## 删除映射

接下来，您需要删除Workfront资产映射。

1. 在Experience Manager中，转到&#x200B;**工具** > **Assets** > **Workfront属性映射**。

1. 选择所有映射，然后单击&#x200B;**删除**。

## 用户权限

所有从Workfront访问AEM Dam的用户都获得了`/content/dam`的读取权限。 如果用户不再需要该权限，您可以删除授予这些用户的权限。

连接器使用系统用户workfront-service操作。 在卸载连接器时，将卸载此项。

>[!NOTE]
>
>如果您使用的是连接器版本2.0.3并且添加了组`workfront-aem-connector-group`，则还需要通过转到&#x200B;**工具** > **安全性** > **组**&#x200B;来删除此组。

## Day CQ链接外部化器

如果您不需要Day CQ Link Externalizer，可以通过转到`/system/console/configMgr`并查找“Day CQ Link Externalizer”将此链接还原为`localhost:4502`。

>[!NOTE]
>
>如果您使用的是Adobe Experience Manager as a Cloud Service，可以通过查看您的项目并在&#x200B;_ui.apps/src/main/content/jcr_root/apps/mysite/config_&#x200B;中查找文件&#x200B;_com.day.cq.commons.impl.ExternalizerImpl.xml_&#x200B;来更改此设置。

![天CQ链接外部化器](assets/Day-CQ-Link-Externalizer.png)

## 卸载连接器包

卸载连接器软件包所需的步骤因您所拥有的Adobe Experience Manager版本而异。

### Adobe Experience Manager On-Premise

如果您使用的是本地Adobe Experience Manager，请转到&#x200B;_crx/packmgr/index.jsp_&#x200B;并查找`workfront-aem-connector.all-<version>.zip`，单击&#x200B;**更多**，然后单击&#x200B;**卸载**。

请检查`/conf`下的内容，以确保已移除所有Workfront创建的文件。

### Adobe Experience Manager as a Cloud Service

对于Adobe Experience Manager as a Cloud Service，您可以从项目的pom.files中删除连接器的依赖项。

## Firewall和Dispatcher

如果不再需要通信，请不要忘记删除已列入白名单的Workfront URL。 此外，连接器使用头apiKey和用户名，该消息已设置为Dispatcher。 这些也可以删除。
