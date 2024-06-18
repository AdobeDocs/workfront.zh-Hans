---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 迁移链接的文件夹和文档
description: 您可以使用该API将链接的文件夹和文档迁移到Adobe Experience Manager Assets。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: aad8f4648a57c93047a1a691d5e608c327d78c1b
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# 迁移链接的文件夹和文档

您可以使用该API将链接的文件夹和文档迁移到Adobe Experience Manager Assets。

## 程序

1. 识别与上一个外部文档存储提供商链接的所有文档和文件夹，记录其Workfront内部文档或文件夹标识符以及任何包含文件夹的文件夹ID。

   >[!NOTE]
   >
   > 您应该检查所有发现的文件夹或文档，以验证它们是否尚未通过新提供商为其创建链接。

1. 按路径在新存储库中查找文档和文件夹，然后在外部系统中查找其身份。

1. 创建内部Workfront ID与新外部存储中的ID的映射。 您需要在以下步骤中使用此项来创建新链接。

1. 在Workfront中创建新文档或文档文件夹链接，通过新外部ID指向新位置的资源。

   1. **文档**：使用新的外部文档提供程序添加现有文档的新版本。
   1. **文件夹**：在相同位置使用相同名称创建新文件夹。

>[!CAUTION]
>
>   请勿删除现有的链接文件夹。 这可能会导致数据丢失。 要从Workfront应用程序中删除旧文件夹链接，请在“设置”区域中禁用自定义文档集成。


## 迁移链接的示例流程

![简化链路流](assets/links-flow-simplified.png)

## API信息

要获取有关Workfront API的更多信息，请参阅此部分 [开发人员文档：文档](https://developer.workfront.com/documents.html).

### 查找所有文档

查找全部 **文档(DOCU)** 链接到 **文档提供商** 之 **providerType** 替换为 **documentProviderId**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[API文档参考](https://developer.workfront.com/documents.html#get-/docu/search)

### 查找所有文件夹

查找全部 **文档文件夹(DOCFDR)** 链接到文档提供程序 **providerType** 替换为 **documentProviderId**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

API文档： (文档文件夹端点当前未包含在developer.workfront.com中)

### 链接文档

链接 **文档(DOCU)** 从 **外部文档提供商** 之 **providerType** 替换为 **documentProviderId**.

>[!IMPORTANT]
>
>文档是临时存储的。 也就是说，您可以访问文档的所有版本。 在创建链接时，您可以指定现有文档ID，因此您只需将新版本写入该文档即可，而数据将托管在新提供商的外部。 此文档ID与在要替换的文档链接上找到的文档ID相同。 这是同一份概念性文件。 您只是指示此新版本的字节存储在其他提供程序中。

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

API文档： (developer.workfront.com上当前未包含内部链接端点)

### 链接文件夹

链接 **文档文件夹(DOCFDR)** 从 **外部文档提供商** 之 **providerType** 替换为 **documentProviderId**.

>[!IMPORTANT]
>
>对于文件夹链接，与文档链接不同，您需要在Workfront中要将新链接放置到的文件夹的“documentFolderId”。 此文件夹很可能与我们复制的链接文件夹相同。

>[!CAUTION]
>
>不会临时存储文件夹。 请勿删除旧文件夹。 在设置区域中禁用自定义文档集成以删除旧文件夹。


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

API文档： (developer.workfront.com上当前未包含内部链接端点)

## 重要术语

* **文档**：Workfront中的数字资源

* **文档文件夹**：Workfront中用于数字资源的容器

* **文档Id**：数字资源的Workfront内部ID

* **文档文件夹ID**：数字资源文件夹的Workfront内部ID

* **文档提供商ID**：与特定文档提供商关联的ID

>[!IMPORTANT]
>
> 对于任何给定的文档提供商类型，客户可以有多个连接的实例。 例如，它们可以链接多个AEM存储库。 或者链接了多个Google Drive实例。 文档提供程序ID指示我们要替换或切换到的连接类型的特定实例。

* **文档存储提供程序类型（也称为“外部集成类型”）**：Workfront支持的文档存储提供程序集成的类型。 通过专用集成或“自定义集成”实现。

* **当前文档存储提供程序类型( providerType)**：

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

* **链接的文档**：在外部文档存储提供商中托管的数字资产。 Workfront将拥有资源的内部“文档ID”，但字节存储在外部。 为了方便实现这一点，Workfront还存储了一个“外部文档ID”，以帮助在远程存储库或存储中定位外部引用的资源。

* **链接的文档文件夹**：在外部文档存储提供商中托管的数字资产的容器。 Workfront将拥有资产的内部“文档文件夹ID”，但字节存储在外部。 为了方便实现这一点，Workfront还存储了一个“外部文档ID”，以帮助在远程存储库或存储中定位外部引用的资源。

* **外部文档ID**：将资源存储在Workfront外部时分配的ID。 Workfront通过此“外部文档标识符”字段将其内部标识符映射到用于在外部系统中查找资产的标识符。 因此，当从新的外部存储链接文档或文件夹时，必须以适当的格式构成新的外部文档标识符，以便外部文档提供者标识新存储库或存储中的文档。

  >[!NOTE]
  >
  > Workfront尚未制定外部文档标识符的标准。 AEM ID使用了新规范，但对于其他ID，外部文档ID可能会采用不同的形式，具体取决于提供商类型。


* **对象类型**：对于本文档而言，这是一个仅用于API的术语。 它是Workfront中您希望与之交互的通用对象类型。 在这种情况下，您将分别与类型为“DOCU”和“DOCFDR”的文档和文件夹进行交互。

* **对象Id**：要与交互的通用对象的内部Workfront标识符。 您将与文档和文件夹进行交互，因此这将是文档ID或文档文件夹ID。
