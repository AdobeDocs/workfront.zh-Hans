---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion Templates管理
description: 如果您是管理员，则有权查看、修改、重命名、发布、批准和删除其他人创建的模板。 您可以从以下位置执行这些操作 [!UICONTROL 模板] 中的页面 [!DNL Adobe Workfront Fusion Administration] 区域。
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 模板管理

如果您是管理员，则有权查看、修改、重命名、发布、批准和删除其他人创建的模板。 您可以从以下位置执行这些操作 [!UICONTROL 模板] 中的页面 [!DNL Adobe Workfront Fusion Administration] 区域。

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
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] （对于工作自动化和集成），[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
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
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是组织的Workfront Fusion管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 视图 [!DNL Workfront Fusion] 管理员模板

要查看包含所有已创建模板及其状态的表，请执行以下操作：

1. 单击 **[!UICONTROL 管理]** 在左侧导航面板中打开 [!UICONTROL 管理] 区域。
1. 单击 **[!UICONTROL 模板]** 左侧导航面板中。

有三个与模板发布状态相关的列。 列中的复选标记表示以下内容：

* **[!UICONTROL 已发布]**：这些模板当前在中可见 [!UICONTROL 团队模板] 选项卡。
* **[!UICONTROL 已请求审批]**：这些模板正在等待您的批准。 它们当前在中可见 [!UICONTROL 团队模板] 选项卡。
* **[!UICONTROL 已批准]**：这些模板已被批准。 它们当前在中可见 [!UICONTROL 公共模板] 选项卡。

>[!NOTE]
>
>同时带有复选标记的模板 [!UICONTROL 已请求审批] 列和中的 [!UICONTROL 已批准] 列已批准并公开，但它们的更新版本正在等待您的批准。

## 编辑 [!DNL Workfront Fusion] 管理员模板

1. 单击 **[!UICONTROL 管理]** 在左侧导航面板中打开 [!UICONTROL 管理] 区域。
1. 单击 **[!UICONTROL 模板]** 左侧导航面板中。
1. 单击 **[!UICONTROL 详细信息]** 位于要编辑的模板的右侧。

您现在可以编辑模板，类似于以非管理员用户身份编辑模板。 但是，在 [!UICONTROL 选项] 在右上角，还有一个附加选项，即为您提供SVG代码的SVG图。 此外，发布过程与标准用户的情况相同，有关更多详细信息，请参阅发布和共享模板一节。

有关可编辑的特定模板选项的信息，请参阅 [在中创建新模板 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

有关发布模板的信息，请参阅 [发布和共享 [!DNL Adobe Workfront Fusion] 模板](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## 批准或取消批准 [!DNL Workfront Fusion] 模板

批准模板可使其在中可见 [!UICONTROL 公共模板] 选项卡，可供所有用户使用。 不批准模板会将其从 [!UICONTROL 公共模板] 选项卡，并仅将其提供给创建它的团队。

1. 单击 **[!UICONTROL 管理]** 在左侧导航面板中打开 [!UICONTROL 管理] 区域。
1. 单击 **[!UICONTROL 模板]** 左侧导航面板中。
1. 如果要批准模板，请单击 **[!UICONTROL 批准]** 模板右侧。
1. 如果要取消批准模板，请单击 **[!UICONTROL 不批准]** 模板右侧。

>[!NOTE]
>
>如果您正在批准之前已批准并编辑的模板，则第二次批准将覆盖原始模板。

## 将方案克隆为模板

作为管理员，您能够将方案克隆为模板。

有关将场景克隆为模板的说明，请参见 [从场景创建模板](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) 在 [在中创建新模板 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
