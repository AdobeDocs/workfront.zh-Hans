---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 自定义默认问题类型
description: 您可以自定义每个默认问题类型的标签，以更好地匹配组织中使用的术语。 问题类型对于自定义问题状态和创建请求队列非常有用。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 自定义默认问题类型

问题类型在以下情况下很有用：

* 自定义问题状态时，如[创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)中所述。
* 创建请求队列时，如[创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)中所述。

您可以自定义每个默认问题类型的标签，以更好地匹配组织中使用的术语。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td><p>新文档： [!UICONTROL Standard]</p>
   或
   <p>当前： [!UICONTROL 计划]</p>
   </td> 
  </tr>
  <tr>
   <td role="rowheader">访问级别配置</td> 
   <td>[!UICONTROL 系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 默认问题类型

如果您具有[!DNL Adobe Workfront] [!UICONTROL 管理员]访问权限，则可以配置和重命名四种默认问题类型：

* **[!UICONTROL 错误报告]**&#x200B;用于跟踪系统中报告的错误。
* **[!UICONTROL 更改顺序]**&#x200B;用于跟踪需要更新或修订的问题。
* **[!UICONTROL 问题]** [!DNL Workfront]中的对象，用于传达计划外工作、出现的问题或为了继续任务而必须解决的事项。
* **[!UICONTROL 请求]**&#x200B;一种问题类型，适用于用户在Workfront中发出请求的请求队列。

![默认问题类型](assets/default-issue-types.png)

## 自定义问题类型

有关自定义问题类型，请考虑以下事项：

* 您可以修改问题类型的标签，但不能更改其功能。
* 无法创建其他问题类型。
* 您无法更改问题类型名称的筛选器值。 因此，如果您在问题报告上创建过滤器，则过滤器的值（键）不反映问题类型的自定义名称。
* 与每个问题类型关联的三个默认状态：[!UICONTROL 新建]、[!UICONTROL 正在进行]和[!UICONTROL 已关闭]。 您无法删除这些状态或从问题类型中删除它们，但可以重命名它们。
* 您可以对每个问题类型的下拉菜单上显示的选项重新排序。

要自定义问题类型，请执行以下操作：

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 项目首选项]** > **[!UICONTROL 状态]**。

1. 单击&#x200B;**[!UICONTROL 问题]**&#x200B;选项卡。
1. 执行以下任一操作：

   * 将鼠标悬停在要自定义的问题类型上，单击最右侧显示的[!UICONTROL 编辑]图标![编辑图标](assets/edit-icon.png)，然后为问题类型键入一个新名称。

     ![自定义问题类型](assets/customize-issue-type.png)

   * 单击[!UICONTROL 问题类型]以列出其关联状态，然后将鼠标悬停在其上方时显示的句柄拖放到该类型上，并按照您希望它们在用户问题&#x200B;**[!UICONTROL 状态]**&#x200B;下拉菜单中显示的顺序进行放置。
