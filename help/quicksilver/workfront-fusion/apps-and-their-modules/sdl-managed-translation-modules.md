---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: SDL管理的翻译模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以将SDL托管翻译帐户连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 1%

---

# [!DNL SDL Managed Translation] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以连接 [!DNL SDL Managed Translation] 帐户到多个第三方应用程序和服务。

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL SDL Managed Translation] 模块

>[!NOTE]
>
>对 [!DNL SDL Managed Translation] is **120秒**.

### 文件

#### [!UICONTROL 下载翻译后的文件]

此模块检索指定项目中包含的单个翻译文件的内容。 如果请求的文件尚未处于“下载”状态，则文件的内容可能尚未完全翻译。 如果文件处于“下载”状态，并且您已成功检索到它，请确保使用将文件标记为完成 `Cancel or Complete File` 方法。

#### [!UICONTROL 上传文件]

此模块允许上传要翻译的文件或将其作为参考材料包含在翻译项目中。 上传必须使用多部分/表单数据提交，并且可以包含多个文件。 您可以指定 `ProjectOptionId` 值，以用于评估已上传的文件。 这可确定您上传的每个文件是翻译的可能候选文件，还是必须作为参考材料进行处理。 就档案而言(`zip `, `rar`, `7z`, `tar` 文件)应用程序会检查存档的内容，并指示整个存档是否可以翻译，或者是否包含可翻译和不可翻译文件的混合内容。

>[!NOTE]
>
>不建议一次上传多个文件，因为它可能会增加任何失败的影响。

#### [!UICONTROL 添加引用文件]

此模块会添加一个引用文件。

### 项目

#### [!UICONTROL 创建项目]

此模块会创建指定的项目。

#### 取消或完成项目

此模块取消或完成指定的项目。 如果项目正在等待下载，则项目将过渡到工作流中的任何最终步骤，并最终移至完成部分。 如果项目正在等待批准或供应商选择被取消。 如果项目处于任何其他状态，则请求将失败。

#### [!UICONTROL 下载项目Zip文件]

此模块将 `zip` 指定项目的已翻译文件文件。

#### [!UICONTROL 阅读项目]

此模块将获取指定的项目。

#### [!UICONTROL 状态为项目]

此模块将获取处于指定状态的所有可用项目。 此方法允许通过指定 `$top`, `$skip`和 `$orderby` 查询参数。

#### [!UICONTROL 获取项目列表]

获取所有项目的简单列表，提供有关每个项目的一般信息。 此方法允许结果为页面，具体方法是：通过指定 `$top`, `$skip`和 `$orderby` 查询参数。

#### [!UICONTROL 搜索项目创建选项]

此模块将获取项目创建选项。

### 其他

#### [!UICONTROL 进行API调用]

此模块执行任意授权的API调用。
