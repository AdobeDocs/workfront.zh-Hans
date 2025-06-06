---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 通过Outlook电子邮件更新现有对象
description: 您可以使用Outlook电子邮件中的信息更新现有项目、任务或问题。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 297eb1c4-ee9f-4bb3-a412-18f23c74b0eb
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# 通过[!DNL Outlook]电子邮件更新现有对象

>[!IMPORTANT]
>
>[Microsoft正在禁用对旧版Exchange联机令牌](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支持，Workfront Outlook加载项当前使用这些令牌进行身份验证。 Microsoft的这一更改已开始影响客户，并将在2025年10月之前继续分阶段推出。
>
>* **在Microsoft完全禁用这些令牌后，Workfront for Microsoft Outlook集成将无法再正常使用。**
>
>作为此更改的一部分，Microsoft已决定更改令牌的重新启用方式。 在&#x200B;**2025年6月30日**&#x200B;之后，管理员将无法再自行重新启用令牌 — 只有Microsoft支持部门可以授予例外。 **在2025年10月1日，将为所有租户关闭旧版令牌。 将不会授予例外。**

您可以通过[!DNL Outlook]电子邮件中的信息更新现有项目、任务或问题。


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

## 通过[!DNL Outlook]电子邮件更新现有对象

1. 在[!DNL Outlook]中，选择包含要包含在[!DNL Adobe Workfront update]中的信息的电子邮件。
1. 单击电子邮件右上角的&#x200B;**[!DNL Workfront]**&#x200B;图标以显示Workfront加载项。\
   您可能需要单击电子邮件右上角的向下箭头才能访问[!DNL Workfront]图标。

1. 单击&#x200B;**[!UICONTROL 菜单]**&#x200B;图标![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png)以显示可用[!DNL Workfront]选项的列表。\


1. 在Workfront **中单击**&#x200B;[!UICONTROL &#x200B;更新]。\
   在将电子邮件另存为任务之前，您可以从电子邮件中更新以下信息：

   * **[!UICONTROL 类型]**：选择要更新的对象类型。 您可以选择&#x200B;**[!UICONTROL 项目]**、**[!UICONTROL 任务]**&#x200B;或&#x200B;**[!UICONTROL 问题]**。 您选择的对象决定了显示在下面的&#x200B;**[!UICONTROL 名称]**&#x200B;字段中的结果。 如果不确定对象的类型，请选择&#x200B;**[!UICONTROL 全部]**&#x200B;以同时搜索项目、任务和问题。

   * **[!UICONTROL 名称]**：开始键入要更新的项目、任务或问题的名称。 当名称出现在下拉列表中时，单击该名称。
   * **[!UICONTROL 更新]**：默认情况下，更新与电子邮件正文相同。 您可以根据需要修改更新。\

     此[!UICONTROL 更新]在Workfront中显示为更新状态。

   * **[!UICONTROL 附件]**：所有电子邮件附件都保存到任务的[!UICONTROL 文档]区域。 您可以在提交更新之前删除任何附件。

1. （可选）单击&#x200B;**[!UICONTROL 包括其他]**，开始键入要包括在更新中的用户的名称，然后在名称出现在下拉列表中时单击该名称。\
   重复此过程以包含其他用户，然后单击&#x200B;**[!UICONTROL 完成]**。\
   默认情况下，无论是否包含要回复的用户，该用户都会收到通知。\

1. （可选）单击&#x200B;**[!UICONTROL 锁定]**&#x200B;图标以将此更新限制在您公司内的用户。 当更新被锁定时，公司外部的用户看不到更新。

   * **[!UICONTROL 已解锁]：**&#x200B;任何有权访问更新所在的项目、任务或问题的用户都可以查看更新。\

     默认情况下，更新处于解锁状态。\
      ![o365_addin_unlock.png](assets/o365-addin-unlock.png)

   * **[!UICONTROL 已锁定]：**&#x200B;只有您公司内的用户可以查看更新。\

     ![o365_addin_lock.png](assets/o365-addin-lock.png)

1. 单击&#x200B;**[!UICONTROL 更新]**。
1. （可选）单击“在Workfront中查看”**&#x200B;**，在[!UICONTROL Outlook]中查看与[!DNL Workfront]集成的更新项。
