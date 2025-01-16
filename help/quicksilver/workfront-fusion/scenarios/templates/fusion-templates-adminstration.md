---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion Templates管理
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: 8163f9f12bb27bbc8adfde34fc1e1f0f8c8be7f9
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]模板管理

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [批准或取消批准“公用”选项卡的模板](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/manage-templates-admin/approve-templates.html)
>* [编辑模板](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/manage-templates-admin/edit-templates.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

如果您是管理员，则有权查看、修改、重命名、发布、批准和删除其他人创建的模板。 您可以从[!DNL Adobe Workfront Fusion Administration]区域的[!UICONTROL 模板]页面执行这些操作。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
    <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]许可证**</td> 
  <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是组织的Workfront Fusion管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 以[!DNL Workfront Fusion]管理员身份查看[!DNL Workfront Fusion]模板

要查看包含所有已创建模板及其状态的表，请执行以下操作：

1. 在左侧导航面板中单击&#x200B;**[!UICONTROL 管理]**&#x200B;以打开[!UICONTROL 管理]区域。

   >[!NOTE]
   >
   >“管理”区域仅对Workfront Fusion管理员可见。

1. 在左侧导航面板中单击&#x200B;**[!UICONTROL 模板]**。

有三个与模板发布状态相关的列。 列中的复选标记表示以下内容：

* **[!UICONTROL 已发布]**：这些模板当前显示在用户界面的[!UICONTROL 团队模板]选项卡中。
* **[!UICONTROL 已请求审批]**：这些模板正在等待您的审批。 它们当前显示在用户界面的[!UICONTROL 团队模板]选项卡中。
* **[!UICONTROL 已批准]**：这些模板已被批准。 它们当前显示在标准用户界面的[!UICONTROL 公共模板]选项卡中。

>[!NOTE]
>
>[!UICONTROL 已请求审批]列和[!UICONTROL 已批准]列中同时带有复选标记的模板已被批准并已公开，但它们的更新版本正在等待您的批准。

## 以管理员身份编辑[!DNL Workfront Fusion]模板

1. 在左侧导航面板中单击&#x200B;**[!UICONTROL 管理]**&#x200B;以打开[!UICONTROL 管理]区域。
1. 在左侧导航面板中单击&#x200B;**[!UICONTROL 模板]**。
1. 单击要编辑的模板右侧的&#x200B;**[!UICONTROL 详细信息]**。

您现在可以编辑模板，类似于以非管理员用户身份编辑模板。 但是，在右上角的[!UICONTROL 选项]中，还有一个附加选项，即为您提供SVG代码的SVG图表。 此外，发布过程与标准用户的情况相同，有关更多详细信息，请参阅发布和共享模板一节。

有关可编辑的特定模板选项的信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)中创建新模板。

有关发布模板的信息，请参阅[Publish和共享 [!DNL Adobe Workfront Fusion] 模板](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md)。

## 批准或不批准[!DNL Workfront Fusion]模板

批准模板可使其在[!UICONTROL 公共模板]选项卡中可见并对所有用户可用。 不批准模板会将其从[!UICONTROL 公共模板]选项卡中删除，并使其仅对创建该模板的团队可用。

1. 在左侧导航面板中单击&#x200B;**[!UICONTROL 管理]**&#x200B;以打开[!UICONTROL 管理]区域。
1. 在左侧导航面板中单击&#x200B;**[!UICONTROL 模板]**。
1. 如果要批准模板，请单击模板右侧的&#x200B;**[!UICONTROL 批准]**。
1. 如果要取消批准模板，请单击模板右侧的&#x200B;**[!UICONTROL 取消批准]**。

>[!NOTE]
>
>如果您要批准之前已批准并编辑的模板，则第二次批准将覆盖原始模板。

## 将方案克隆为模板

作为管理员，您能够将方案克隆为模板。

有关将方案克隆为模板的说明，请参阅[在 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)中创建新模板中的[从方案创建模板](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario)
