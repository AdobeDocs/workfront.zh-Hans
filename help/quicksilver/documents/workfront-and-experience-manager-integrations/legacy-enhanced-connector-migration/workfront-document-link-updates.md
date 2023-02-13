---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 迁移链接的文件夹和文档
description: 您可以使用API将链接的文件夹和文档迁移到Adobe Experience Manager Assets。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# 迁移链接的文件夹和文档

您可以使用API将链接的文件夹和文档迁移到Adobe Experience Manager Assets。

## 过程

1. 识别与以前的外部文档存储提供程序链接的所有文档和文件夹，并注明其Workfront内部文档或文件夹标识符，以及任何包含文件夹的文件夹ID。

   >[!NOTE]
   >
   > 您应该检查所有已发现的文件夹或文档，以确认它们尚未与新提供商一起为它们创建链接。

1. 在新存储库中按路径找到文档和文件夹，然后在外部系统中查找其标识。

1. 创建内部Workfront ID到新外部存储中ID的映射。 您需要此参数才能在以下步骤中创建新链接。

1. 在Workfront中创建新文档或文档文件夹链接，通过其新外部ID指向新位置中的资源。

   1. **文档**:使用新的外部文档提供程序添加现有文档的新版本。
   1. **文件夹**:在同一位置使用相同名称创建新文件器。

>[!CAUTION]
>
>   请勿删除现有的链接文件夹。 这可能会导致数据丢失。 要从Workfront应用程序中删除旧文件夹链接，请在“设置”区域禁用自定义文档集成。


## 迁移链接的示例流程

![简化链接流](assets/links-flow-simplified.png)

## API信息

有关此部分中Workfront API的更多信息，请参阅 [开发人员文档：文档](https://developer.workfront.com/documents.html).

### 查找所有文档

全部查找 **文档(DOCU)** 链接到 **文档提供程序** of **providerType** with **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[API文档参考](https://developer.workfront.com/documents.html#get-/docu/search)

### 查找所有文件夹

全部查找 **文档文件夹(DOCFDR)** 链接到的文档提供程序 **providerType** with **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

API文档：（developer.workfront.com上当前未涵盖的文档文件夹端点）

### 链接文档

链接 **文档(DOCU)** 从 **外部文档提供程序** of **providerType** with **documentProviderID**.

>[!IMPORTANT]
>
>文档会临时存储。 即，您有权访问文档的所有版本。 创建链接时，您可以指定现有的文档ID，因此您只是在该文档中写入新版本，数据将在外部托管在新提供程序中。 此文档ID与您正在替换的文档链接上的文档ID相同。 是同样的概念性文档。 您只是表示此新版本的字节与其他提供程序一起存储。

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

API文档：（developer.workfront.com上当前未涵盖的内部链接端点）

### 链接文件夹

链接 **文档文件夹(DOCFDR)** 从 **外部文档提供程序** of **providerType** with **documentProviderID**.

>[!IMPORTANT]
>
>对于文件夹链接，与文档链接不同，您需要将新链接放入Workfront中的文件夹的“documentFolderId”。 这很可能与要复制的链接文件夹是相同的父文件夹。

>[!CAUTION]
>
>文件夹不会临时存储。 请勿删除旧文件夹。 在设置区域中禁用自定义文档集成以删除旧文件夹。


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

API文档：（developer.workfront.com上当前未涵盖的内部链接端点）

## 重要术语

* **文档**:Workfront中的数字资产

* **文档文件夹**:Workfront中的数字资产容器

* **文档ID**:Workfront数字资产的内部ID

* **文档文件夹ID**:Workfront数字资产文件夹的内部ID

* **文档提供程序ID**:与特定文档提供程序关联的ID

>[!IMPORTANT]
>
> 对于任何给定的文档提供商类型，客户可能具有多个连接的实例。 例如，他们可能已关联多个AEM存储库。 或链接多个Google驱动器实例。 文档提供程序ID指示要替换或切换到的连接类型的特定实例。

* **文档存储提供程序类型（也称为“外部集成类型”）**:Workfront支持的文档存储提供程序集成类型。 通过专用集成或“自定义集成”。

* **当前文档存储提供程序类型(providerType)**:

   ```
   ATTASK
   BOX
   GOOGLE
   SHAREPOINT
   WEBDAM
   WORKFRONTDAM
   INFERNO
   WIDEN
   DROPBOX
   DROPBOX_BUSINESS
   ONEDRIVE
   QUIP
   WEBHOOKS
   AEM
   MOCK
   ```

* **链接的文档**:在外部文档存储提供程序中托管的数字资产。 Workfront将具有其自己的资产内部“文档ID”，但字节是存储在外部的。 为了实现此目的，Workfront还存储了“外部文档ID”，以帮助在远程存储库或存储中查找外部引用的资源。

* **链接的文档文件夹**:在外部文档存储提供程序中托管的数字资产容器。 Workfront将具有其自己的资产内部“文档文件夹ID”，但字节是存储在外部。 为了实现此目的，Workfront还存储了“外部文档ID”，以帮助在远程存储库或存储中查找外部引用的资源。

* **外部文档ID**:资产存储在Workfront外部时分配的ID。 Workfront会通过此“外部文档标识符”字段，将其内部标识符映射到用于在外部系统中查找资产的标识符。 因此，当从新外部存储库链接文档或文件夹时，必须合成新的外部文档标识符，其格式为外部文档提供者在新存储库或存储中标识文档的适当格式。

   >[!NOTE]
   >
   > Workfront尚没有外部文档标识符的标准。 AEM ID正在使用新规范，但对于其他ID，外部文档ID可能采用不同的表单，具体取决于提供商类型。


* **对象类型**:对于本文档而言，这是仅用于API的术语。 它是Workfront中要与之交互的通用对象类型。 在这种情况下，您将与分别具有“DOCU”和“DOCFDR”类型的文档和文件夹进行交互。

* **对象ID**:要与之交互的通用对象的内部Workfront标识符。 您将与文档和文件夹进行交互，以便这将分别为文档ID或文档文件夹ID。
