---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 从Outlook电子邮件创建 [!DNL Adobe Workfront] 请求
description: 您可以在Outlook中通过电子邮件创建 [!DNL Adobe Workfront] 请求。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# 从[!UICONTROL Outlook]电子邮件创建[!DNL Adobe Workfront]请求

>[!IMPORTANT]
>
>[Microsoft正在禁用对旧版Exchange联机令牌](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支持，Workfront Outlook加载项当前使用这些令牌进行身份验证。 Microsoft的这一更改已开始影响客户，并将在2025年10月之前继续分阶段推出。
>
>* **在Microsoft完全禁用这些令牌后，Workfront for Microsoft Outlook集成将无法再正常使用。**
>
>作为此更改的一部分，Microsoft已决定更改令牌的重新启用方式。 在&#x200B;**2025年6月30日**&#x200B;之后，管理员将无法再自行重新启用令牌 — 只有Microsoft支持部门可以授予例外。 **在2025年10月1日，将为所有租户关闭旧版令牌。 将不会授予例外。**

您可以在Outlook中通过电子邮件创建[!DNL Adobe Workfront]请求。

基于电子邮件创建[!DNL Workfront]请求时，默认情况下请求中包含电子邮件的内容（包括主题和正文）。

>[!NOTE]
>
>无法从共享[!UICONTROL Outlook]邮箱创建[!DNL Workfront]请求。

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

## 通过[!DNL Outlook]电子邮件创建请求

要从[!DNL Outlook]创建[!DNL Workfront]请求，请执行以下操作：

1. 选择包含要包含在[!DNL Workfront]请求中的信息的电子邮件。
1. 单击电子邮件右上角的&#x200B;**[!DNL Workfront]**&#x200B;图标以显示Workfront加载项。\
   您可能需要单击电子邮件右上角的向下箭头才能访问[!DNL Workfront]图标。

1. 单击&#x200B;**[!UICONTROL 菜单]**&#x200B;图标![o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png)以显示可用[!DNL Workfront]选项的列表。

1. 单击&#x200B;**[!UICONTROL 提交请求]**。
1. 在&#x200B;**[!UICONTROL 选择请求类型]**&#x200B;字段中，选择要提交请求的请求队列。

1. 指定以下信息：\
   可用字段可能会因请求队列的设置方式而异。 有关可能字段的完整列表和说明，请参阅[创建并提交 [!DNL Adobe Workfront] 请求](../../manage-work/requests/create-requests/create-submit-requests.md)文章。

   * **[!UICONTROL 主题]：**&#x200B;为请求指定主题。 默认情况下，使用电子邮件主题。
   * **[!UICONTROL 描述]：**&#x200B;为请求指定描述。 默认情况下，会使用电子邮件正文。
   * **[!UICONTROL 文档]：**&#x200B;附加要包含在请求中的任何文档。 您可以通过拖放或单击&#x200B;**[!UICONTROL 选择文件]**&#x200B;并浏览和选择文档来附加文档。\

     默认情况下，附加到电子邮件的任何文档都会包含在请求中。

1. 单击&#x200B;**[!UICONTROL 提交请求]**。\
   请求在指定的请求队列中提交到[!DNL Workfront]。

1. （可选）导航回[!DNL Outlook]，然后选择原始电子邮件。\
   在[!DNL Workfront]加载项面板顶部，注意包含链接的确认，表明电子邮件已作为请求添加到Workfront。 该链接包含转换日期。\
