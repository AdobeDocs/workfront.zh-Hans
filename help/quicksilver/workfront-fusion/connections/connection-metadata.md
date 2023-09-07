---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-2-0
title: Adobe Workfront Fusion中的连接元数据
description: 除了Adobe Workfront许可证之外，Adobe Workfront Fusion还需要Adobe Workfront Fusion许可证。
author: Becky
feature: Workfront Fusion
source-git-commit: 3a7983279a38c30cb58078d129ea22dee137d9a5
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Adobe Workfront Fusion中的连接元数据

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 需要 [!DNL Adobe Workfront Fusion] 除了许可证外， [!DNL Adobe Workfront] 许可证。

并非所有连接都相同。 了解连接之间的差异对于了解其业务环境非常重要。 Fusion使用元数据来标识连接的重要属性。

创建新连接时可以设置连接元数据。 这些属性位于用于设置连接的同一对话框中：

![连接元数据](assets/connection-metadata-setup.png)

Fusion用户可以从“连接”区域查看和编辑连接。

![连接区域中的连接元数据](assets/connections-area-metadata.png)

## 环境类型

生产和非生产系统均可使用Fusion连接。 了解差异对于保护生产环境非常重要。 请注意，环境类型与其他连接元数据一样，仅用于提供信息。 用户仍然负责准确地设置此属性。

## 身份验证类型

Fusion连接可用于服务帐户和个人帐户。 当场景自动变为Fusion时，使用服务帐户进行身份验证。 个人帐户是基于特定人员的身份验证。 使用的身份验证类型取决于方案的要求。 个人帐户应用于自动用户操作。 例如，如果Fusion场景自动批准特定人员，则身份验证类型应该适用于该人员。 否则，Fusion将充当Fusion，并且类型应为“服务帐户”。

请注意，与其他连接元数据一样，类型仅用于提供信息。 用户仍然负责手动准确设置此属性。

有关身份验证类型的更多信息，请参阅 [身份验证](https://developer.adobe.com/developer-console/docs/guides/authentication/) 《Adobe身份验证指南》中的。



