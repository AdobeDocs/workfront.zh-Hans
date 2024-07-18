---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Publish和共享 [!DNL Adobe Workfront Fusion] 模板
description: 创建模板后，您的模板将可供所有团队成员使用。 如果要与团队外部的人员共享模板，则必须先发布该模板。
author: Becky
feature: Workfront Fusion
exl-id: aaa59a1e-aa16-41f5-9f56-ce0615c1b685
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# Publish和共享[!DNL Adobe Workfront Fusion]模板

创建模板后，您的模板将可供所有团队成员使用。 如果要与团队外部的人员共享模板，则必须先发布该模板。

有关创建模板的信息，请参阅[在Adobe Workfront Fusion中创建新模板](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

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
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]许可证**</td> 
  <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 先决条件

必须先创建模板，然后才能共享模板。

## Publish和[!DNL Adobe Workfront Fusion]模板

1. 在左侧导航面板中，单击&#x200B;**[!UICONTROL 模板]**。
1. 单击&#x200B;**[!UICONTROL 团队模板]**&#x200B;选项卡。
1. 单击模板的名称。
1. 单击屏幕右上角的&#x200B;**[!UICONTROL Publish]**&#x200B;按钮。

## 共享[!DNL Workfront Fusion]模板

发布模板后，即可共享该模板。

1. （视情况而定）如果您需要可共享链接，请单击&#x200B;**[!UICONTROL 共享公共链接]**。

   >[!NOTE]
   >
   >您可以与任何所需人员共享此链接。 模板本身停留在[!UICONTROL 团队模板]选项卡中并且不是公共的。

1. （视情况而定）如果希望将模板公开，请单击&#x200B;**[!UICONTROL 请求审批]**&#x200B;以将其发送给管理员以供审批。

   >[!NOTE]
   >
   >* 模板获得批准后，即会公开。 [!UICONTROL 公共模板]在所有[!DNL Workfront Fusion]用户的[!UICONTROL 公共模板]选项卡中可见，无论组织或团队如何。
   >* 您的管理员不会收到通过电子邮件接收模板以进行审阅的通知。 如果批准情况紧急，请直接联系管理员。


## 模板状态

您可以在模板名称下查看模板页面上的状态

可以使用以下状态：

* **[!UICONTROL 私有]**：此模板仅对模板作者及其团队可见。
* **[!UICONTROL 已发布]**：此模板仅对模板作者及其团队可见。 您可以发送已发布的模板以供审批，并复制可共享链接。
* **[!UICONTROL 已批准]**：此模板在[!UICONTROL 公共模板]选项卡中对所有Workfront Fusion用户可见。 您可以通过单击屏幕右上角的[!UICONTROL 选项]来复制可共享链接。

您还可以从[!UICONTROL 团队模板]选项卡中检查状态。 如果模板已发布，则模板名称的右侧将显示一个图标。

* **眼睛图标**：模板已发布，仅对团队可见，并且未发送审批请求。
* **黄色复选标记图标**：模板已发布，仅对团队可见，并且已发送审批请求。
* **绿色复选标记图标**：模板已发布并已公开。 它在[!UICONTROL 公共模板]选项卡中对任何Workfront Fusion用户可见。 它还在[!UICONTROL 团队模板]选项卡中可见，并且模板作者或其团队成员仍然可以编辑它。

没有图标的模板具有[!UICONTROL 私有]状态。 它们未发布，仅对团队可见。
