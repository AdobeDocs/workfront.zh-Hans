---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在中创建新模板 [!DNL Adobe Workfront Fusion]
description: 您可以在中创建新方案模板 [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# 在中创建新模板 [!DNL Adobe Workfront Fusion]

您可以在中创建新方案模板 [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>创建新模板之前，您可以检查 [!UICONTROL 公共模板] 选项卡以确保要创建的模板不可用。

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

## 创建新模板

您可以在类似于构建场景的流程中构建模板。 Fusion管理员还可以从现有场景创建模板。

* [构建模板](#build-a-template)
* [从场景创建模板](#create-a-template-from-a-scenario)

### 构建模板

1. 单击 **[!UICONTROL 模板]** ![](assets/fusion-template-icon.png) 左侧导航面板中。
1. 单击 **[!UICONTROL 创建新模板]** 在右上角。
1. （可选）通过替换默认模板来重命名模板 **[!UICONTROL 新模板名称]** 左上角。
1. （可选）要更改模板的语言，请单击 **[!UICONTROL 设置模板]** ![](assets/fusion-scenario-settings-icon.png) 并从语言下拉列表中选择语言。

   >[!IMPORTANT]
   >
   >语言选择对应于系统设置中可用的语言，仅涉及公共模板的名称及其描述。 保存模板后，无法更改模板语言。

1. （可选）要输入模板的说明，请单击 **[!UICONTROL 设置模板]** ![](assets/fusion-scenario-settings-icon.png) 并输入说明。
1. 使用创建标准方案时所用的相同方式添加应用程序、模块和工具。

   要向模块添加上下文帮助，请参阅 [设置 [!UICONTROL 向导] 功能](#set-up-wizard-functionality) 本文章中。

   有关构建方案的详细信息，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >如果您的模板包含需要添加连接、凭据或其他隐私敏感信息的模块，则不会与模板用户共享此信息。

1. （可选）单击 **[!UICONTROL 运行一次]** 以测试您的模板。
1. 单击 **[!UICONTROL 保存]** 图标 ![](assets/save-icon.png).

>[!NOTE]
>
>通过保存您的模板，您可以使其对所有团队成员可见。 如果您希望在团队外部可以访问模板，则需要发布该模板，然后使用共享链接，或请求管理员批准并发布该模板。

### 从场景创建模板

>[!NOTE]
>
>您必须是Fusion管理员才能从场景中创建模板。

1. 打开要从中创建方案的方案的方案详细信息页面。
1. 单击 **管理员** 在页面的右上角附近下拉菜单。
1. 选择 **克隆为模板**.

   该方案将被复制到新模板页面中。
1. （可选）通过替换默认模板来重命名模板 **[!UICONTROL 新模板名称]** 左上角。
1. （可选）要更改模板的语言，请单击 **[!UICONTROL 设置模板]** ![](assets/fusion-scenario-settings-icon.png) 并从语言下拉列表中选择语言。

   >[!IMPORTANT]
   >
   >语言选择对应于系统设置中可用的语言，仅涉及公共模板的名称及其描述。 保存模板后，无法更改模板语言。

1. （可选）要输入模板的说明，请单击 **[!UICONTROL 设置模板]** ![](assets/fusion-scenario-settings-icon.png) 并输入说明。
1. 使用与编辑标准场景时相同的方式编辑应用程序、模块和工具。

   要向模块添加上下文帮助，请参阅 [设置 [!UICONTROL 向导] 功能](#set-up-wizard-functionality) 本文章中。

   >[!NOTE]
   >
   >如果您的模板包含需要添加连接、凭据或其他隐私敏感信息的模块，则不会与模板用户共享此信息。

1. （可选）单击 **[!UICONTROL 运行一次]** 以测试您的模板。
1. 单击 **[!UICONTROL 保存]** 图标 ![](assets/save-icon.png).

## 设置 [!UICONTROL 向导] 功能 {#set-up-wizard-functionality}

此 [!DNL Workfront Fusion template] [!UICONTROL 向导] 允许您为模板的将来用户提供与模块中使用的特定字段相关的说明或信息。

1. 单击添加到模板的模块，以查看模块的字段。
1. 找到要添加位置的字段 [!UICONTROL 向导] 信息，并启用 **[!UICONTROL 在向导中使用]** 为那个场地。
1. 将您希望对用户可见的信息输入到 [!UICONTROL 帮助] 字段。
1. （可选）要允许用户在使用模板时查看此文本，请启用 **[!UICONTROL 用作默认值]**.
1. 对要为其提供信息的每个字段重复步骤2-4。
1. 单击 **[!UICONTROL 确定]** 以保存更改并关闭模块。
