---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 创建 [!DNL Adobe Workfront] Outlook电子邮件中的请求
description: 您可以创建 [!DNL Adobe Workfront] 来自Outlook电子邮件的请求。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# 创建 [!DNL Adobe Workfront] 来自 [!UICONTROL Outlook] 电子邮件

您可以创建 [!DNL Adobe Workfront] 来自Outlook电子邮件的请求。

创建 [!DNL Workfront] 基于电子邮件的请求，默认情况下，电子邮件的内容（包括主题和正文）包含在请求中。

>[!NOTE]
>
>您无法创建 [!DNL Workfront] 来自共享的请求 [!UICONTROL Outlook] 邮箱。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Work]、[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 先决条件

您的 [!DNL Workfront] 管理员必须启用 [!DNL Outlook for Office] with [!DNL Workfront] ，以便您使用此集成。

## 从 [!DNL Outlook] 电子邮件

创建 [!DNL Workfront] 请求来源 [!DNL Outlook]:

1. 选择包含要包含在 [!DNL Workfront] 请求。
1. 单击 **[!DNL Workfront]** 图标来显示Workfront加载项。\
   您可能需要单击电子邮件右上角的向下箭头才能访问 [!DNL Workfront] 图标。

1. 单击 **[!UICONTROL 菜单]** 图标以显示可用列表 [!DNL Workfront] 选项。

   ![o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png)

1. 单击 **[!UICONTROL 提交请求]**.
1. 在 **[!UICONTROL 选择请求类型]** 字段中，选择要在其中提交请求的请求队列。

   ![o365_addin_submitrequest.png](assets/o365-addin-submitrequest.png)

1. 指定以下信息：\
   根据请求队列的设置方式，可用字段可能会有所不同。 有关可能字段的完整列表和说明，请参阅 [创建和提交 [!DNL Adobe Workfront] 请求](../../manage-work/requests/create-requests/create-submit-requests.md) 文章。

   * **[!UICONTROL 主题]:** 指定请求的主题。 默认情况下，会使用电子邮件主题。
   * **[!UICONTROL 描述]:** 为请求指定描述。 默认情况下，会使用电子邮件正文。
   * **[!UICONTROL 文档]:** 附加要包含在请求中的任何文档。 您可以通过拖放或单击 **[!UICONTROL 选择文件]** 浏览并选择文档。\

      默认情况下，附加到电子邮件的任何文档都会包含在请求中。

1. 单击 **[!UICONTROL 提交请求]**.\
   请求已提交到 [!DNL Workfront]，位于指定的请求队列中。

1. （可选）导航回 [!DNL Outlook]，然后选择原始电子邮件。\
   在 [!DNL Workfront] 加载项面板中，请注意带有链接的确认，即电子邮件已作为请求添加到Workfront。 链接包括转换日期。\
   ![outlook_submitted_as_a_request.png](assets/outlook-submitted-as-a-request-350x130.png)
