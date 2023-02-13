---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 自定义默认问题类型
description: 您可以自定义每个默认问题类型的标签，以更好地匹配您组织中使用的术语。 问题类型对于自定义问题状态和创建请求队列非常有用。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# 自定义默认问题类型

问题类型在以下情况下非常有用：

* 自定义问题状态时，如 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* 创建请求队列时，如 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

您可以自定义每个默认问题类型的标签，以更好地匹配您组织中使用的术语。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 默认问题类型

如果 [!DNL Adobe Workfront] [!UICONTROL 管理员] 访问，您可以配置和重命名四种默认问题类型：

* **[!UICONTROL 错误报告]** 用于跟踪系统中报告的错误。
* **[!UICONTROL 更改顺序]** 用于跟踪需要更新或修订的问题。
* **[!UICONTROL 问题]** 中的对象 [!DNL Workfront] 传达计划外工作、出现问题或必须解决以便继续执行任务的信息。
* **[!UICONTROL 请求]** 适用于用户在Workfront中发出请求的请求队列的问题类型。

![](assets/default-issue-types.png)

## 自定义问题类型

请考虑以下有关自定义问题类型的信息：

* 您可以修改问题类型的标签，但无法更改其函数。
* 您无法创建其他问题类型。
* 无法更改问题类型名称的过滤器值。 因此，如果在问题报表上创建过滤器，则过滤器（键）的值不会反映问题类型的自定义名称。
* 每种问题类型都关联了三种默认状态： [!UICONTROL 新建], [!UICONTROL 正在进行]和 [!UICONTROL 已关闭]. 您无法删除这些状态或从问题类型中删除它们，但可以对它们进行重命名。
* 您可以对每个问题类型的下拉菜单中显示的选项进行重新排序。

要自定义问题类型，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 项目首选项]** > **[!UICONTROL 状态]**.

1. 单击 **[!UICONTROL 问题]** 选项卡。
1. 执行以下任一操作：

   * 将鼠标悬停在要自定义的问题类型上，单击 [!UICONTROL 编辑] 图标 ![](assets/edit-icon.png) ，然后为问题类型键入新名称。

      ![](assets/customize-issue-type.png)

   * 单击 [!UICONTROL 问题类型] 要列出其关联状态，请将鼠标悬停在手柄上时显示的手柄上，然后按您希望手柄在用户问题中显示的顺序拖放这些手柄 **[!UICONTROL 状态]** 下拉菜单。
