---
product-area: projects
navigation-topic: use-the-home-area
title: 从主页区域创建工作项
description: 从主页区域创建工作项
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 9db6e509-ea6a-493a-9d86-21a163da1915
source-git-commit: 3793f68faf2ec0a8050f8f0c6e06a32579b43879
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# 从主页区域创建工作项

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From Courtney: Need to rename)</p>
-->

您可以从中创建工作项 [!UICONTROL 主页] 区域。 您可以自行创建个人任务、向其他用户请求工作或向特定项目添加任务。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[！UICONTROL Worker]</p> <p>注意：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[！UICONTROL Edit]或更高版本对任务的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 创建个人任务

您可以在中创建仅供您使用的个人任务 [!UICONTROL 主页] 区域：

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) 图标，然后单击 **[!UICONTROL 主页]**.
1. 单击 **[!UICONTROL 新建任务]** > **[!UICONTROL 个人]**.

   ![](assets/creating-work-items-new-task-personal-nwe-350x228.png)

1. 在 **[!UICONTROL 名称]** 字段中，指定任务的名称。
1. （可选）单击 **[!UICONTROL 选择日期]**，然后选择任务的到期日期。 这会将 [!UICONTROL 计划完成日期] 完成任务。\
   您可以更改 **[!UICONTROL 计划完成日期]** 单击右侧面板中的日期或编辑 **[!UICONTROL 完成日期为]** 任务中的直接日期。

1. 单击 **[!UICONTROL 创建]** 以保存任务。\
   任务已分配给您，并且可在以下位置找到： [!UICONTROL 主页] 区域。

>[!NOTE]
>
>* 创建个人任务时，该任务存储在不可搜索的“隐藏”项目中 [!UICONTROL Workfront]. 该项目名为“&lt;用户名>‘的任务>”。 “用户名”是创建任务的用户的全名。 只有当您单击中的个人任务时，才能访问此项目。 [!UICONTROL 主页] 区域，例如，任务的痕迹导航。
>
>* 与常规项目任务不同，个人任务在Workfront界面中可见的字段集有限，并且不会影响任何项目的时间表或进度。 将个人任务重新分配给另一个用户会将所有任务字段添加到个人任务，但该任务仍然保留在创建该任务的用户的个人项目上。
>
>* 如果要将个人任务纳入常规工作流，我们建议您创建一个项目，并将任何个人任务移动到该项目。
>
> ![[!UICONTROL 个人任务项目]](assets/createworkitems-personal--project-350x105.png)

## 从其他用户请求工作

您可以直接从主页区域向其他用户请求工作。 当按照本节所述向其他用户请求工作时，任务将作为请求显示在用户的“主页”区域中，直到用户单击为止 **[!UICONTROL 处理此项工作]**.

要向其他用户请求工作，请执行以下操作： [!UICONTROL 主页] 区域：

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) 图标，然后单击 **[!UICONTROL 主页]**.
1. 单击 **[!UICONTROL 新建任务]**，然后选择 **[!UICONTROL 请求]**.

   ![](assets/creating-work-items-new-task-request-nwe-350x283.png)

1. 在 **[!UICONTROL 名称]** 字段中，指定任务的名称。
1. 在 **[!UICONTROL 分配给]** 字段中，开始键入要分配的用户、团队或角色的名称，然后在名称出现在下拉菜单中时单击该名称。
1. 在 [!UICONTROL 添加为] 下拉菜单，选择添加任务还是问题。
1. 单击 **[!UICONTROL 选择日期]**，然后选择任务的到期日期和时间。
1. 单击 **[!UICONTROL 创建]** 以保存任务。\
   任务将作为工作请求显示在中 [!UICONTROL 主页] 指定用户的区域。

## 将任务或问题添加到项目

您可以直接从主页区域将任务或问题添加到现有项目：

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) 图标，然后单击 **主页**.
1. 单击 **[!UICONTROL 新建任务]**，然后选择 **[!UICONTROL 项目任务]**.

   ![](assets/creating-work-items-new-project-task-nwe-350x358.png)

1. 在 **[!UICONTROL 名称]** 字段中，指定任务或问题的名称。
1. 在 **[!UICONTROL 分配给]** 字段中，开始键入要分配的用户、团队或角色的名称，然后在名称出现在下拉菜单中时单击该名称。
1. 开始键入要在其中创建任务或问题的项目的名称，然后在名称出现在下拉菜单中时单击该名称。

   >[!IMPORTANT]
   >
   >任务或问题出现在 [!UICONTROL 工作列表] 仅当项目 [!UICONTROL 状态] 设置为 [!UICONTROL 当前].

1. （视情况而定）要创建问题，请选择 **[!UICONTROL 问题]** 从 **[!UICONTROL 添加为]** 下拉菜单。 默认情况下， **[!UICONTROL 任务]** 已选中。

1. 单击 **[!UICONTROL 选择日期]**，然后选择任务的到期日期和时间。
1. 单击 **[!UICONTROL 创建]** 以保存任务。
