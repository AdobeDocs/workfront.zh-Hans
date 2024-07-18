---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: 移动敏捷故事
description: 您可以将敏捷故事移动到不同的迭代（对于Scrum团队）或积压（对于Kanban和Scrum团队）。
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 移动敏捷故事

您可以将敏捷故事移动到不同的迭代（对于Scrum团队）或积压（对于Kanban和Scrum团队）。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[！UICONTROL Worker]或更高版本</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[！UICONTROL Manage]对文章的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 将故事从迭代或Kanban展示板移动到积压

1. 转到包含要移至积压的项目故事的迭代或Kanban展示板。
1. 单击页面顶部的迭代标题。
1. 在&#x200B;**[!UICONTROL 故事]**&#x200B;选项卡上，选择要移动的故事。
1. 单击&#x200B;**[!UICONTROL 更多]** > **[!UICONTROL 移至]**。

   将显示&#x200B;**[!UICONTROL 移动故事]**&#x200B;对话框。

   ![移动故事对话框](assets/iteration-story-move.png)

1. 选择&#x200B;*team_name*&#x200B;的积压。\
   在上例中，团队名称为&#x200B;**Marketing.**

1. 单击&#x200B;**[!UICONTROL 移动故事]**。

## 将故事移动到其他迭代

您可以为Scrum团队将故事移动到其他迭代。

>[!NOTE]
>
>**[!UICONTROL 移至]**&#x200B;选项不适用于开发周期中的父故事。 您只能将子任务移动到另一个迭代。

1. 转到包含要移动的故事的迭代。
1. 单击页面顶部的迭代标题。
1. 在&#x200B;**[!UICONTROL 故事]**&#x200B;选项卡上，选择要移动的故事。
1. 单击&#x200B;**[!UICONTROL 更多]** > **[!UICONTROL 移至]**。

   将显示&#x200B;**[!UICONTROL 移动故事]**&#x200B;对话框。

   ![移动故事对话框](assets/iteration-story-move.png)

1. 选择&#x200B;**[!UICONTROL 其他迭代]**，然后在下拉菜单中，选择要将文章移动到的迭代。

   >[!NOTE]
   >
   >工作项[!UICONTROL 计划开始日期]和[!UICONTROL 计划完成日期]受[!UICONTROL 编辑团队]页面上的设置影响。 有关信息，请参阅[配置Scrum](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)一文中的[[!UICONTROL 配置]将工作项添加到迭代时，日期的应用方式](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)部分。

1. 单击&#x200B;**[!UICONTROL 移动故事]**。
