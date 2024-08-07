---
product-area: projects
navigation-topic: use-the-home-area
title: 从主页区域创建工作项
description: 您可以从[!UICONTROL 主页]区域创建工作项。 您可以为自己创建个人任务、向其他用户请求工作或向特定项目添加任务。
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: 9db6e509-ea6a-493a-9d86-21a163da1915
source-git-commit: 644e2487dae0d3b2f7931660fb8e6ed68e6b8b93
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# 从主页区域创建工作项

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From Courtney: Need to rename)</p>
-->

您可以从[!UICONTROL 主页]区域创建工作项。 您可以为自己创建个人任务、向其他用户请求工作或向特定项目添加任务。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[！UICONTROL Worker]</p> <p><b>注释</b></p> 
   <p>如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[！UICONTROL Edit]或更高版本对任务的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 创建个人任务

您可以在[!UICONTROL 主页]区域创建仅供您使用的个人任务：

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. 单击&#x200B;**[!UICONTROL 新建任务]** > **[!UICONTROL 个人]**。

   ![](assets/creating-work-items-new-task-personal-nwe-350x228.png)

1. 在&#x200B;**[!UICONTROL 名称]**&#x200B;字段中，指定任务的名称。
1. （可选）单击&#x200B;**[!UICONTROL 选择日期]**，然后选择任务到期的日期。 这会设置任务的[!UICONTROL 计划完成日期]。\
   您可以通过单击右侧面板中的日期或编辑&#x200B;**[!UICONTROL 直接在任务中完成]**&#x200B;日期来更改&#x200B;**[!UICONTROL 规划完成日期]**。

1. 单击&#x200B;**[!UICONTROL 创建]**&#x200B;以保存任务。\
   该任务已分配给您，并且在[!UICONTROL 主页]区域可用。

>[!NOTE]
>
>* 创建个人任务时，该任务存储在[!UICONTROL Workfront]中不可搜索的“隐藏”项目中。 该项目名为“&lt;用户名>‘的任务>”。 “用户名”是创建任务的用户的全名。 仅当从任务的痕迹导航单击[!UICONTROL 主页]区域中的个人任务时，才能访问此项目，例如。
>
>* 与常规项目任务不同，个人任务在Workfront界面中可见的字段集有限，并且不会影响任何项目的时间线或进度。 将个人任务重新分配给另一个用户会将所有任务字段添加至个人任务，但该任务仍保留在创建该任务的用户的个人项目中。
>
>
>* 仅当个人任务记录了小时数或将它们固定到时间表时，才会显示在时间表上。 仅当为任务记录了小时数时，您才可以将个人任务固定到时间表。 有关详细信息，请参阅[记录时间](../../../timesheets/create-and-manage-timesheets/log-time.md)。
> 
>* 如果要将个人任务变成常规工作流的一部分，我们建议您创建项目并将任何个人任务移动到项目中。
>
> 个人任务的![[!UICONTROL 项目]](assets/createworkitems-personal--project-350x105.png)

## 请求另一个用户的工作

您可以直接从“主页”区域向其他用户请求工作。 如本节所述，当您向其他用户请求工作时，该任务将作为请求显示在用户的“主页”区域中，直到用户单击&#x200B;**[!UICONTROL 处理该任务]**&#x200B;为止。

要从[!UICONTROL 主页]区域向其他用户请求工作，请执行以下操作：

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. 单击&#x200B;**[!UICONTROL 新建任务]**，然后选择&#x200B;**[!UICONTROL 请求]**。

   ![](assets/creating-work-items-new-task-request-nwe-350x283.png)

1. 在&#x200B;**[!UICONTROL 名称]**&#x200B;字段中，指定任务的名称。
1. 在&#x200B;**[!UICONTROL 分配给]**&#x200B;字段中，开始键入要分配的用户、团队或角色的名称，然后在名称出现在下拉菜单中时单击该名称。
1. 在[!UICONTROL 添加为]下拉菜单中，选择添加任务还是问题。
1. 单击&#x200B;**[!UICONTROL 选择日期]**，然后选择任务到期的日期和时间。
1. 单击&#x200B;**[!UICONTROL 创建]**&#x200B;以保存任务。\
   该任务将作为工作请求显示在指定用户的[!UICONTROL 主页]区域中。

## 将任务或问题添加到项目

您可以直接从主页区域将任务或问题添加到现有项目：

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png)，然后单击&#x200B;**主页**。
1. 单击&#x200B;**[!UICONTROL 新建任务]**，然后选择&#x200B;**[!UICONTROL 项目任务]**。

   ![](assets/creating-work-items-new-project-task-nwe-350x358.png)

1. 在&#x200B;**[!UICONTROL 名称]**&#x200B;字段中，指定任务或问题的名称。
1. 在&#x200B;**[!UICONTROL 分配给]**&#x200B;字段中，开始键入要分配的用户、团队或角色的名称，然后在名称出现在下拉菜单中时单击该名称。
1. 开始键入要在其中创建任务或问题的项目名称，然后在名称出现在下拉菜单中时单击该名称。

   >[!IMPORTANT]
   >
   >仅当项目[!UICONTROL 状态]设置为[!UICONTROL 当前]时，任务或问题才会出现在[!UICONTROL 工作列表]中。

1. （视情况而定）要创建问题，请从&#x200B;**[!UICONTROL 添加为]**&#x200B;下拉菜单中选择&#x200B;**[!UICONTROL 问题]**。 默认情况下，已选择&#x200B;**[!UICONTROL 任务]**。

1. 单击&#x200B;**[!UICONTROL 选择日期]**，然后选择任务到期的日期和时间。
1. 单击&#x200B;**[!UICONTROL 创建]**&#x200B;以保存任务。
