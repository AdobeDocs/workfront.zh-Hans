---
title: Intacct模块
description: Intacct模块
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: fa1aa943-fbda-4eb4-bfa1-ab94a56785a7
source-git-commit: 9a4a847b542783845a3f896ec4e35d5efc7c122b
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---

# Intacct模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用Intact的工作流，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## 先决条件

要使用Intacct模块，您必须拥有Intacct帐户。

## 将Intacct连接到Workfront Fusion

### 授权 [!DNL Workfront Fusion] 在Intacct中进行更改

之前 [!DNL Workfront Fusion] 可以连接到 [!DNL Intacct]，则必须对其进行授权。

在您的Intacct帐户中，导航到 **[!UICONTROL 公司]** 选项卡。

1. 单击 **公司信息**.
1. 导航到 **安全性** 选项卡。
1. 单击 [!UICONTROL 编辑] 在右上角
1. 选择Web服务授权。
1. 单击加号图标
1. 输入AzuquaMPP作为sender_id。
1. （可选）输入连接的描述

### 在中设置连接 [!DNL Workfront Fusion] {#set-up-a-connection-in-workfront-fusion}

您可以创建与 [!DNL Intacct] 直接从内部帐户 [!DNL Intacct] 模块。

1. 在任意Intacct模块中，单击 **[!UICONTROL 添加]** 连接字段旁边。
1. 输入Intacct凭据

   * 公司 ID
   * 用户 ID
   * 密码

1. 单击 **[!UICONTROL 继续]** 创建连接，然后返回到模块。

## 集成模块及其字段

配置 [!DNL Intacct] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除这些字段外，可能还会显示其他Intacct字段，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL 进行自定义API调用]](#make-a-custom-api-call)
* [[!UICONTROL 搜索记录]](#search-records)

### [!UICONTROL 进行自定义API调用] {#make-a-custom-api-call}

通过此操作模块，您可以对 [!DNL Intacct] API。 这样，您就可以创建数据流自动化，而另一个数据流无法实现 [!DNL Intacct] 模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>连接</p> </td> 
   <td> <p>有关将Intacct帐户连接到 [!DNL Workfront Fusion] 2.0，请参阅 <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">在Workfront Fusion中设置连接</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">正文XML</td> 
   <td> <p>仅将XML包含在主体内。 请求会自动包含身份验证标头。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜索记录]

此搜索模块可检索与特定搜索条件匹配的记录列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>连接</p> </td> 
   <td> <p>有关将Intacct帐户连接到 [!DNL Workfront Fusion] 2.0，请参阅 <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">在Workfront Fusion中设置连接</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td> <p>选择要搜索的记录类型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>搜索条件</p> </td> 
   <td> 
    <ul> 
     <li> <p>选择要搜索的字段</p> </li> 
     <li> <p>选择要用于搜索的运算符</p> </li> 
     <li> <p>输入要搜索的值</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">结果集</td> 
   <td>选择是要返回所有匹配记录，还是仅返回第一个匹配记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">限制</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">排序方式</td> 
   <td>选择要按对结果进行排序的字段。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">顺序</td> 
   <td>选择是升序排序还是降序排序。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">输出</td> 
   <td> <p>选择要包含在此模块的输出包中的信息。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">区分大小写</td> 
   <td>启用此选项，可使查询区分大小写。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">查询专用实体</td> 
   <td>启用此选项，以允许模块搜索专用实体。</td> 
  </tr> 
 </tbody> 
</table>
