---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 发布和共享 [!DNL Adobe Workfront Fusion] 模板
description: 创建模板后，您的模板将可供所有团队成员使用。 如果要与团队外部的人员共享模板，则必须先发布该模板。
author: Becky
feature: Workfront Fusion
exl-id: aaa59a1e-aa16-41f5-9f56-ce0615c1b685
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# 发布和共享 [!DNL Adobe Workfront Fusion] 模板

创建模板后，您的模板将可供所有团队成员使用。 如果要与团队外部的人员共享模板，则必须先发布该模板。

有关创建模板的信息，请参阅 [在Adobe Workfront Fusion中创建新模板](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

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
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] （对于工作自动化和集成），[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
   </td>    </tr> 
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

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 先决条件

必须先创建模板，然后才能共享模板。

## 发布 [!DNL Adobe Workfront Fusion] 模板

1. 在左侧导航面板中，单击 **[!UICONTROL 模板]**.
1. 单击 **[!UICONTROL 团队模板]** 选项卡。
1. 单击模板的名称。
1. 单击 **[!UICONTROL Publish]** 按钮来打开屏幕。

## 共享 [!DNL Workfront Fusion] 模板

发布模板后，即可共享该模板。

1. （视情况而定）如果您需要可共享链接，请单击 **[!UICONTROL 共享公共链接]**.

   >[!NOTE]
   >
   >您可以根据需要与任何人共享此链接。 模板本身保留在 [!UICONTROL 团队模板] 制表符且不公开。

1. （视情况而定）如果您希望将模板公开，请将其发送给管理员以供审批，方法是单击 **[!UICONTROL 请求审批]**.

   >[!NOTE]
   >
   >* 模板获得批准后，即会公开。 [!UICONTROL 公共模板] 在中可见 [!UICONTROL 公共模板] 选项卡（全部） [!DNL Workfront Fusion] 用户，无论组织或团队如何。
   >* 您的管理员不会收到通过电子邮件查看模板的通知。 如果批准情况紧急，请直接联系管理员。


## 模板状态

您可以在模板名称下检查模板页面上的状态

可以使用以下状态：

* **[!UICONTROL 私人]**：此模板仅对模板作者及其团队可见。
* **[!UICONTROL 已发布]**：此模板仅对模板作者及其团队可见。 您可以发送已发布的模板以供审批，并复制可共享链接。
* **[!UICONTROL 已批准]**：此模板对中的所有Workfront Fusion用户可见 [!UICONTROL 公共模板] 选项卡。 您可以通过单击 [!UICONTROL 选项] 在屏幕右上角。

您还可以从以下位置检查状态 [!UICONTROL 团队模板] 选项卡。 如果模板已发布，则模板名称的右侧将显示一个图标。

* **“眼睛”图标**：模板已发布，仅对团队可见，并且未发送审批请求。
* **黄色复选标记图标**：模板已发布，仅对团队可见，并且已发送审批请求。
* **绿色复选标记图标**：模板已发布并已公开。 它对于中的任何Workfront Fusion用户都可见 [!UICONTROL 公共模板] 选项卡。 它也仍然显示在 [!UICONTROL 团队模板] 选项卡，并且模板作者或其团队成员仍可以编辑它。

没有图标的模板具有 [!UICONTROL 私人] 状态。 它们未发布，仅对团队可见。
