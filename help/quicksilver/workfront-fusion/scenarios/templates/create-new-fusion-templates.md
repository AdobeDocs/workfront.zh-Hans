---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在 [!DNL Adobe Workfront Fusion]中创建新模板
description: 您可以在 [!DNL Adobe] Workfront Fusion中创建新场景模板。
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: f3f34e807228b299c0570e63bdf329f4e20e0340
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中创建新模板

您可以在[!DNL Adobe] Workfront Fusion中创建新场景模板。

>[!TIP]
>
>创建新模板之前，您可以检查[!UICONTROL 公共模板]选项卡，以确保要创建的模板尚不可用。

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

## 创建新模板

您可以在一个与构建方案类似的过程中构建模板。 Fusion管理员还可以从现有方案创建模板。

* [构建模板](#build-a-template)
* [从场景创建模板](#create-a-template-from-a-scenario)

### 构建模板

1. 在左侧导航面板中单击&#x200B;**[!UICONTROL 模板]** ![](assets/fusion-template-icon.png)。
1. 单击右上角的&#x200B;**[!UICONTROL 创建新模板]**。
1. （可选）通过替换左上角的默认&#x200B;**[!UICONTROL 新模板名称]**&#x200B;来重命名模板。
1. （可选）要更改模板的语言，请单击&#x200B;**[!UICONTROL 设置模板]** ![](assets/fusion-scenario-settings-icon.png)，然后从“语言”下拉列表中选择语言。

   >[!IMPORTANT]
   >
   >语言选择对应于系统设置中可用的语言，仅涉及公共模板的名称及其描述。 保存模板后，无法更改模板语言。

1. （可选）要输入模板的描述，请单击&#x200B;**[!UICONTROL 设置模板]** ![](assets/fusion-scenario-settings-icon.png)并输入描述。
1. 按照创建标准方案时所用的相同方式添加应用程序、模块和工具。

   若要向模块添加上下文帮助，请参阅本文中的[设置[!UICONTROL 向导]功能](#set-up-wizard-functionality)。

   有关构建方案的详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md)中创建方案。

   >[!NOTE]
   >
   >如果您的模板包含需要添加连接、凭据或其他隐私敏感信息的模块，则不会与模板用户共享此信息。

1. （可选）单击&#x200B;**[!UICONTROL 运行一次]**&#x200B;以测试您的模板。
1. 单击&#x200B;**[!UICONTROL 保存]**&#x200B;图标![](assets/save-icon.png)。

>[!NOTE]
>
>通过保存模板，您可以使其对所有团队成员可见。 如果您希望可以在团队外部访问模板，则必须提交请求以批准和发布模板。 该请求将进入Adobe Workfront进行审批，在获得批准后，您团队之外的其他人可以访问该模板。
>
>有关发布模板的信息，请参阅[Publish和共享 [!DNL Adobe Workfront Fusion] 模板](/help/quicksilver/workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md)。

### 从场景创建模板

>[!NOTE]
>
>您必须是Fusion管理员才能从场景创建模板。

1. 打开要从中创建方案的方案的方案详细信息页面。
1. 单击页面右上角附近的&#x200B;**管理员**&#x200B;下拉菜单。
1. 选择&#x200B;**克隆作为模板**。

   方案将被复制到新模板页面中。
1. （可选）通过替换左上角的默认&#x200B;**[!UICONTROL 新模板名称]**&#x200B;来重命名模板。
1. （可选）要更改模板的语言，请单击&#x200B;**[!UICONTROL 设置模板]** ![](assets/fusion-scenario-settings-icon.png)，然后从“语言”下拉列表中选择语言。

   >[!IMPORTANT]
   >
   >语言选择对应于系统设置中可用的语言，仅涉及公共模板的名称及其描述。 保存模板后，无法更改模板语言。

1. （可选）要输入模板的描述，请单击&#x200B;**[!UICONTROL 设置模板]** ![](assets/fusion-scenario-settings-icon.png)并输入描述。
1. 使用与编辑标准场景相同的方式编辑应用程序、模块和工具。

   若要向模块添加上下文帮助，请参阅本文中的[设置[!UICONTROL 向导]功能](#set-up-wizard-functionality)。

   >[!NOTE]
   >
   >如果您的模板包含需要添加连接、凭据或其他隐私敏感信息的模块，则不会与模板用户共享此信息。

1. （可选）单击&#x200B;**[!UICONTROL 运行一次]**&#x200B;以测试您的模板。
1. 单击&#x200B;**[!UICONTROL 保存]**&#x200B;图标![](assets/save-icon.png)。

## 设置[!UICONTROL 向导]功能 {#set-up-wizard-functionality}

[!DNL Workfront Fusion template] [!UICONTROL 向导]允许您向模板的将来用户提供与模块中使用的特定字段相关的说明或信息。

1. 单击添加到模板的模块以查看模块的字段。
1. 找到要添加[!UICONTROL 向导]信息的字段，并为该字段启用&#x200B;**[!UICONTROL 在向导中使用]**。
1. 在[!UICONTROL 帮助]字段中输入您希望用户可见的信息。
1. （可选）要允许用户在使用模板时查看此文本，请启用&#x200B;**[!UICONTROL 使用作为默认值]**。
1. 对要为其提供信息的每个字段重复步骤2 - 4。
1. 单击&#x200B;**[!UICONTROL 确定]**&#x200B;以保存更改并关闭模块。
