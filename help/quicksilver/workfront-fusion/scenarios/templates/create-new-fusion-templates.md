---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在中创建新模板 [!DNL Adobe Workfront Fusion]
description: 您可以在 [!DNL Adobe] Workfront融合。
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 在中创建新模板 [!DNL Adobe Workfront Fusion]

您可以在 [!DNL Adobe] Workfront融合。

>[!TIP]
>
>在创建新模板之前，您可以检查 [!UICONTROL 公共模板] 选项卡，以确保要创建的模板尚未可用。

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

## 创建新模板

1. 单击 **[!UICONTROL 模板]** ![](assets/fusion-template-icon.png) 中。
1. 单击 **[!UICONTROL 创建新模板]** 中。
1. （可选）通过替换默认模板 **[!UICONTROL 新模板名称]** 中。
1. （可选）要更改模板的语言，请单击 **[!UICONTROL 设置模板]** ![](assets/fusion-scenario-settings-icon.png) 并从语言下拉列表中选择语言。

   >[!IMPORTANT]
   >
   >“语言”选项与系统设置中提供的语言相对应，只涉及公共模板的名称及其说明。 保存模板后，便无法更改模板语言。

1. （可选）要输入模板的说明，请单击 **[!UICONTROL 设置模板]** ![](assets/fusion-scenario-settings-icon.png) 并输入描述。
1. 以与创建标准方案时相同的方式添加应用程序、模块和工具。

   要向模块添加上下文帮助，请参阅 [设置 [!UICONTROL 向导] 功能](#set-up-wizard-functionality) 在本文中。

   有关构建方案的更多信息，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >如果您的模板包含需要添加连接、凭据或其他隐私敏感信息的模块，则此信息不会与模板用户共享。

1. （可选）单击 **[!UICONTROL 运行一次]** 来测试模板。
1. 单击 **[!UICONTROL 保存]** 图标 ![](assets/save-icon.png).

>[!NOTE]
>
>通过保存模板，可使模板对所有团队成员可见。 如果您希望模板可在团队外部访问，则需要发布该模板，然后使用共享链接，或请求管理员批准和发布模板。

## 设置 [!UICONTROL 向导] 功能 {#set-up-wizard-functionality}

的 [!DNL Workfront Fusion template] [!UICONTROL 向导] 允许您为模板的未来用户提供与模块中使用的特定字段相关的说明或信息。

1. 单击添加到模板的模块可查看模块的字段。
1. 找到要添加的字段 [!UICONTROL 向导] 信息和启用 **[!UICONTROL 在向导中使用]** 对于该字段。
1. 在 [!UICONTROL 帮助] 字段。
1. （可选）要允许用户在使用模板时查看此文本，请启用 **[!UICONTROL 用作默认值]**.
1. 对要提供信息的每个字段重复步骤2-4。
1. 单击 **[!UICONTROL 确定]** 保存更改并关闭模块。
