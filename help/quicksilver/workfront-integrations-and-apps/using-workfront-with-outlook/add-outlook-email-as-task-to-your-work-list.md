---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 将Outlook电子邮件作为任务添加到您的工作列表
description: 您可以将 [!DNL Outlook] 电子邮件转换为 [!DNL Adobe Workfront] 任务。 在转换电子邮件后，该任务会显示在主页区域的工作列表中。
author: Becky
feature: Workfront Integrations and Apps
exl-id: fcd02116-ffeb-43d3-8541-5e30e6cfdc5e
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---

# 将[!DNL Outlook]电子邮件作为任务添加到您的工作列表

>[!IMPORTANT]
>
>[Microsoft正在禁用对旧版Exchange联机令牌](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支持，Workfront Outlook加载项当前使用这些令牌进行身份验证。 Microsoft的这一更改已开始影响客户，并将在2025年10月之前继续分阶段推出。
>
>* **在Microsoft完全禁用这些令牌后，Workfront for Microsoft Outlook集成将无法再正常使用。**
>
>作为此更改的一部分，Microsoft已决定更改令牌的重新启用方式。 在&#x200B;**2025年6月30日**&#x200B;之后，管理员将无法再自行重新启用令牌 — 只有Microsoft支持部门可以授予例外。 **在2025年10月1日，将为所有租户关闭旧版令牌。 将不会授予例外。**



您可以将[!DNL Outlook]电子邮件转换为[!DNL Adobe Workfront]任务。 电子邮件转换后，任务将在[!UICONTROL 主页]区域的[!UICONTROL 工作]列表中可用。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL 工作]，[!UICONTROL 计划]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 先决条件

您的[!DNL Workfront]管理员必须使用[!DNL Workfront]启用[!DNL Outlook for Office]，然后才能使用此集成。

## 将[!DNL Outlook]电子邮件作为任务添加到您的工作列表

1. 选择[!DNL Outlook]中要转换为任务的电子邮件。
1. 单击电子邮件右上角的&#x200B;**[!DNL Workfront]**&#x200B;图标以显示[!DNL Workfront]加载项。\
   您可能需要单击电子邮件右上角的向下箭头才能访问[!DNL Workfront]图标。

1. 单击&#x200B;**[!UICONTROL 菜单]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png)图标以显示可用[!DNL Workfront]选项的列表。\


1. 单击&#x200B;**[!UICONTROL 添加到工作]**。\

1. 取消选择&#x200B;**[!UICONTROL 添加到项目]**&#x200B;字段。
1. （可选）在保存为任务之前，您可以从电子邮件中更新以下信息：

   * **[!UICONTROL 任务名称]：**&#x200B;默认情况下，任务名称与电子邮件主题相同。 您可以根据需要修改任务名称。
   * **[!UICONTROL 描述]：**&#x200B;默认情况下，描述与电子邮件正文相同。 您可以根据需要修改描述。
   * **[!UICONTROL 附件]：**&#x200B;任何电子邮件附件都会保存到任务的[!UICONTROL 文档]区域。 在将电子邮件另存为任务之前，您可以删除任何附件。

1. 单击&#x200B;**[!UICONTROL 添加]**。\
   任务已添加到主页区域中的[!UICONTROL 工作列表]，但没有提交日期。

1. （可选）单击“在Workfront中查看”**&#x200B;**&#x200B;以在新选项卡中显示[!DNL Workfront]应用程序中的任务。

1. （可选）导航回[!DNL Outlook]，然后选择原始电子邮件。\
   在[!DNL Workfront]加载项面板顶部，注意包含链接的确认，表明电子邮件已作为任务添加到Workfront。 该链接包含转换日期。\
