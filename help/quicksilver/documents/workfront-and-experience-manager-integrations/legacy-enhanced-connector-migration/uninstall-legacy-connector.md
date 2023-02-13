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
source-wordcount: '424'
ht-degree: 0%

---

# 使用Adobe Experience Manager旧版连接器卸载Workfront

您必须将Workfront与Adobe Experience Manager旧版连接器卸载到连接Workfront和Adobe Experience Manager Assets的最新本机集成as a Cloud Service。

## 取消订阅Workfront

1. 打开Adobe Experience Manager。
1. 在Experience Manager中，转到 **工具** > **Cloud Services** > **Workfront集成配置**.
1. 选择您的配置（默认情况下为全局工作流），然后单击 **属性**.
   ![退订workfront](assets/unsubscribe-from-workfront.png)
1. 禁用文档、注释和元数据同步。 标签应当已禁用。
这将删除Workfront中的订阅，并允许用户使用Day CQ Link Externalizer中定义的相同url创建新订阅。

## 删除Workfront集成配置

删除订阅后，现在可以安全地删除Workfront集成配置。

1. 打开配置，然后选择 **删除**.
   ![删除配置](assets/delete-wf-configuration.png)

## 删除映射

接下来，您需要删除Workfront属性映射。

1. 在Experience Manager中，转到 **工具** > **资产** > **Workfront属性映射**.

1. 选择所有映射，然后单击 **删除**.

## 用户权限

所有从Workfront访问AEM Dam的用户都有权读取 `/content/dam`. 如果用户不再需要该权限，您可以删除授予该用户的权限。

连接器使用系统用户工作前端服务操作。 卸载连接器时，此操作将被卸载。

>[!NOTE]
>
>如果您使用的是连接器版本2.0.3并添加了组 `workfront-aem-connector-group`，则还需要通过以下路径删除该页面： **工具** > **安全性** > **群组**.

## Day CQ链接外部器

如果不需要Day CQ Link Externalizer，可以将此链接还原回 `localhost:4502` 通过 `/system/console/configMgr` 和正在查找“Day CQ Link Externalizer”。

>[!NOTE]
>
>如果您使用的是Adobe Experience Manager as a Cloud Service，则可以通过查看项目并查找文件来更改此设置 _com.day.cq.commons.impl.ExternalizerImpl.xml_ in _ui/apps/src/main/content/jcr_root/apps/mysite/config_.

![Day CQ链接外部器](assets/Day-CQ-Link-Externalizer.png)

## 卸载连接器软件包

卸载连接器软件包所需的步骤因您拥有的Adobe Experience Manager版本而异。

### Adobe Experience Manager内部部署

如果您使用的是内部部署的Adobe Experience Manager，请转到 _crx/packmgr/index.jsp_，并查找 `workfront-aem-connector.all-<version>.zip`，单击 **更多** 然后 **卸载**.

请查看下 `/conf` 以确保删除所有Workfront创建的文件。

### Adobe Experience Manager as a Cloud Service

对于Adobe Experience Manager as a Cloud Service，您可以从项目的pom.files中删除连接器的依赖项。

## 防火墙和调度程序

如果不再需要通信，请勿忘记删除已列入白名单的Workfront URL。 此外，连接器还使用设置为调度程序的标头apiKey和用户名。 这些也可以删除。
