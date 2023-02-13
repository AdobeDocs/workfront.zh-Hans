---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 发布和共享 [!DNL Adobe Workfront Fusion] 模板
description: 创建模板时，模板将可供所有团队成员使用。 如果要与团队外的人员共享模板，则必须先发布该模板。
author: Becky
feature: Workfront Fusion
exl-id: aaa59a1e-aa16-41f5-9f56-ce0615c1b685
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# 发布和共享 [!DNL Adobe Workfront Fusion] 模板

创建模板时，模板将可供所有团队成员使用。 如果要与团队外的人员共享模板，则必须先发布该模板。

有关创建模板的信息，请参阅 [在Adobe Workfront Fusion中创建新模板](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化） </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 先决条件

必须先创建模板，才能共享。

## 发布 [!DNL Adobe Workfront Fusion] 模板

1. 在左侧导航面板中，单击 **[!UICONTROL 模板]**.
1. 单击 **[!UICONTROL 团队模板]** 选项卡。
1. 单击模板的名称。
1. 单击 **[!UICONTROL 发布]** 按钮。

## 共享 [!DNL Workfront Fusion] 模板

发布模板后，即可共享该模板。

1. （视情况而定）如果您想要可共享链接，请单击 **[!UICONTROL 共享公共链接]**.

   >[!NOTE]
   >
   >您可以与任何想要的人共享此链接。 模板本身位于 [!UICONTROL 团队模板] 选项卡，且不是公共的。

1. （视情况而定）如果您希望模板变为公用模板，请通过单击 **[!UICONTROL 请求批准]**.

   >[!NOTE]
   >
   >* 模板一旦获得批准，便会变为公用。 [!UICONTROL 公共模板] 在 [!UICONTROL 公共模板] 选项卡 [!DNL Workfront Fusion] 用户，无论是组织还是团队。
   >* 系统不会向您的管理员发送有关通过电子邮件接收要审阅的模板的通知。 如果紧急，请直接与管理员联系。



## 模板状态

您可以在模板名称下检查模板页面上的状态

以下状态可用：

* **[!UICONTROL 私有]**:此模板仅对模板作者及其团队可见。
* **[!UICONTROL 已发布]**:此模板仅对模板作者及其团队可见。 您可以发送已发布的模板以供审批，并复制可共享链接。
* **[!UICONTROL 已批准]**:此模板对中的所有Workfront Fusion用户均可见 [!UICONTROL 公共模板] 选项卡。 您可以通过单击 [!UICONTROL 选项] 中。

您还可以从 [!UICONTROL 团队模板] 选项卡。 如果模板已发布，则其名称右侧将显示一个图标。

* **眼睛图标**:模板已发布，且仅对团队可见，且未发送批准请求。
* **黄色复选标记图标**:模板已发布，且仅对团队可见，并且已发送批准请求。
* **绿色复选标记图标**:该模板已发布并公开。 它对中的任何Workfront Fusion用户都可见 [!UICONTROL 公共模板] 选项卡。 此外，它也仍显示在 [!UICONTROL 团队模板] 选项卡，并且模板作者或其团队成员仍可以对其进行编辑。

没有图标的模板 [!UICONTROL 私有] 状态。 它们未发布，且仅供团队查看。
