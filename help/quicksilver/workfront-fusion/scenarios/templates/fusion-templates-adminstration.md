---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion模板管理
description: 如果您是管理员，则有权查看、修改、重命名、发布、批准和删除他人创建的模板。 您可以从 [!UICONTROL 模板] 页面 [!DNL Adobe Workfront Fusion Administration] 的上界。
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: bcca026e193e66cfb92ab9a0fb1aaf1eeb6892fb
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 模板管理

如果您是管理员，则有权查看、修改、重命名、发布、批准和删除他人创建的模板。 您可以从 [!UICONTROL 模板] 页面 [!DNL Adobe Workfront Fusion Administration] 的上界。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

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
    <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化） </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是贵组织的Workfront Fusion管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 查看 [!DNL Workfront Fusion] 管理员模板

要查看所有已创建模板及其状态的表，请执行以下操作：

1. 单击 **[!UICONTROL 管理]** 在左侧导航面板中打开 [!UICONTROL 管理] 的上界。
1. 单击 **[!UICONTROL 模板]** 中。

模板发布状态有三列。 列中的复选标记表示以下内容：

* **[!UICONTROL 已发布]**:这些模板当前在 [!UICONTROL 团队模板] 选项卡。
* **[!UICONTROL 请求批准]**:这些模板正在等待您批准。 它们当前在 [!UICONTROL 团队模板] 选项卡。
* **[!UICONTROL 已批准]**:这些模板已获得批准。 它们当前在 [!UICONTROL 公共模板] 选项卡。

>[!NOTE]
>
>在 [!UICONTROL 请求批准] 列和 [!UICONTROL 已批准] 列已获得批准并公开，但有较新版本的列正在等待您批准。

## 编辑 [!DNL Workfront Fusion] 管理员模板

1. 单击 **[!UICONTROL 管理]** 在左侧导航面板中打开 [!UICONTROL 管理] 的上界。
1. 单击 **[!UICONTROL 模板]** 中。
1. 单击 **[!UICONTROL 详细信息]** 的子菜单。

您现在可以编辑模板，与以非管理员用户身份编辑模板类似。 但是，在 [!UICONTROL 选项] 在右上角，还有一个其他选项 — SVG图，为您提供SVG代码。 此外，发布过程与标准用户的过程相同，有关更多详细信息，请参阅发布和共享模板一节。

有关可编辑的特定模板选项的信息，请参阅 [在中创建新模板 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

有关发布模板的信息，请参阅 [发布和共享 [!DNL Adobe Workfront Fusion] 模板](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## 批准或不批准 [!DNL Workfront Fusion] 模板

批准模板后，该模板将显示在 [!UICONTROL 公共模板] 选项卡，并可供所有用户使用。 不批准模板会将其从 [!UICONTROL 公共模板] 选项卡，并仅将其提供给创建该选项卡的团队。

1. 单击 **[!UICONTROL 管理]** 在左侧导航面板中打开 [!UICONTROL 管理] 的上界。
1. 单击 **[!UICONTROL 模板]** 中。
1. 如果要批准模板，请单击 **[!UICONTROL 批准]** 的位置。
1. 如果要不批准模板，请单击 **[!UICONTROL 不批准]** 的位置。

>[!NOTE]
>
>如果您批准之前已批准并编辑的模板，则第二次批准将覆盖原始模板。

## 克隆模板方案

作为管理员，您可以克隆模板方案。

有关将方案克隆为模板的说明，请参阅 [根据方案创建模板](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) in [在中创建新模板 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
