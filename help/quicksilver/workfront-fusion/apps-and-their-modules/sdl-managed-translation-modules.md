---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: SDL托管翻译模块
description: 在 [!DNL Adobe Workfront Fusion] 方案，您可以将SDL Managed Translation帐户连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# [!DNL SDL Managed Translation] 模块

在 [!DNL Adobe Workfront Fusion] 方案，您可以将 [!DNL SDL Managed Translation] 帐户到多个第三方应用程序和服务。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL SDL Managed Translation] 模块

>[!NOTE]
>
>对的调用的操作超时 [!DNL SDL Managed Translation] 是 **120秒**.

### 文件

#### [!UICONTROL 下载已翻译文件]

此模块检索指定项目中包含的单个已翻译文件的内容。 如果所请求的文件尚未处于Downland状态，则可能尚未完全翻译该文件的内容。 如果文件处于“下载”状态，并且您已成功检索到文件，请确保使用 `Cancel or Complete File` 方法。

#### [!UICONTROL 上传文件]

此模块允许上传文件以供翻译或作为参考材料包含在翻译项目中。 上载必须使用多部分/表单数据提交，并且可以包含多个文件。 您指定 `ProjectOptionId` 用于评估已上传的文件。 这会确定您上传的每个文件是翻译的可能候选文件，还是必须作为参考材料处理。 在档案方面(`zip `， `rar`， `7z`， `tar` 文件)，应用程序会检查存档的内容，并指示存档是否可以整个翻译，或者是否包含可翻译和不可翻译的混合文件。

>[!NOTE]
>
>不建议一次上传多个文件，因为这样可能会增加任何失败的影响。

#### [!UICONTROL 添加参考文件]

此模块添加一个参考文件。

### 项目

#### [!UICONTROL 创建项目]

此模块创建指定的项目。

#### 取消或完成项目

此模块取消或完成指定的项目。 如果项目正在等待下载，则项目会完成工作流中的任何最终步骤，并最终移动完成。 如果项目正在等待审批或供应商选择被取消。 如果项目处于任何其他状态，则请求将失败。

#### [!UICONTROL 下载项目Zip]

此模块获得 `zip` 指定项目的已翻译文件的文件。

#### [!UICONTROL 读取项目]

此模块获取指定的项目。

#### [!UICONTROL 获取处于状态的项目]

此模块获取所有处于指定状态的可用项目。 此方法允许通过指定 `$top`， `$skip`、和 `$orderby` 查询参数。

#### [!UICONTROL 获取项目列表]

获取所有项目的简单列表，提供有关每个项目的一般信息。 此方法允许将结果设置为页面，方法是指定 `$top`， `$skip`、和 `$orderby` 查询参数。

#### [!UICONTROL 搜索项目创建选项]

此模块获取项目创建选项。

### 其他

#### [!UICONTROL 进行API调用]

此模块执行任意授权的API调用。
