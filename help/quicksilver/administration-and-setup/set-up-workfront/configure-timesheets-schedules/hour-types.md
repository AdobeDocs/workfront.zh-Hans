---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 管理小时类型
description: 您可以将小时类型与小时条目关联。 小时类型是用于定义小时条目的标签。
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 1%

---

# 管理小时类型

<!--Audited: 07/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

您可以将小时类型与小时条目关联。 小时类型是用于定义小时条目的标签。

有两组小时类型：

* **特定项目小时类型**：此时间已记录到项目、任务和问题。 特定项目小时类型可以与[!DNL Adobe Workfront]中的任何时间条目关联，您可以在其中记录项目、任务和问题的时间。

  在[!DNL Workfront]中记录时间时，可用的项目特定小时类型取决于在系统、项目和用户级别设置的配置选项。

  以下特定于项目的默认小时类型始终可用：

   * 项目时间
   * 任务时间
   * 问题时间

  [!DNL Workfront]管理员确定哪些项目特定的小时类型可用，如[定义小时类型和可用性](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)中所述。

  >[!NOTE]
  >
  >如果您在[!DNL Workfront]系统中启用了任何特定于项目的小时类型，则必须在系统中的每个项目上至少启用一种特定于项目的小时类型。 您无法在系统级别启用特定于项目的小时类型，并且在项目级别没有可用的特定于项目的小时类型。

* **常规小时类型**：常规小时不能与项目、任务或问题相关联，并且直接登录到时间表。

有关记录小时数并将其与小时类型关联的信息，请参阅[记录时间](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront]计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>新文档： [！UICONTROL Standard]</p>
   <p>当前： [！UICONTROL计划]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别</td> 
   <td>[！UICONTROL系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 内置小时类型

Workfront附带一组内置小时类型。 这些小时类型无法编辑，也无法隐藏。

[!DNL Workfront]附带的小时类型包括：

* **[!UICONTROL 病假时间]**：不能与项目、任务或问题的小时条目关联的常规小时类型。 病假小时数不能计为收入。
* **[!UICONTROL 休假时间]**：不能与项目、任务或问题的小时条目关联的常规小时类型。 休假时间不能计为收入。
* **[!UICONTROL 常规开销]**：不能与项目、任务或问题的小时条目关联的常规小时类型。 但是，它可以在项目计划流程中计为收入。
* **[!UICONTROL 项目时间]**：只能与项目小时条目关联的常规小时类型。
* **[!UICONTROL 任务时间]**：只能与任务的小时条目关联的常规小时类型。
* **[!UICONTROL 问题时间]**：只能与问题的小时条目关联的常规小时类型。

## 创建小时类型

作为[!DNL Workfront]管理员，您可以在系统和项目级别为组织创建新的小时类型。 在系统和项目级别创建小时类型后，用户可以定义哪些小时类型可用于特定项目和用户。 有关详细信息，请参阅[定义小时类型和可用性](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

要创建新小时类型，请执行以下操作：

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 时间表和小时数]** > **[!UICONTROL 小时类型]**。

1. 单击&#x200B;**[!UICONTROL 新建小时类型].**
1. 在&#x200B;**[!UICONTROL 新小时类型]**&#x200B;表单中指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL名称]</td> 
      <td>为您的新小时键入一个易于在系统中识别的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL描述]</td> 
      <td>添加对小时类型的描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL作用域]</td> 
      <td> <p>通过在下拉菜单中选择正确的范围来定义小时类型是常规小时类型还是特定于项目的小时类型。</p> <p>常规小时类型仅在时间表中可见，且不能与项目、任务或问题相关联。</p> <p><b>重要信息</b>：如果您有一个自定义小时类型，该类型是[！UICONTROL项目特定的]，然后您将其更改为[！UICONTROL常规]，则所有现有的任务、问题和项目小时数都将设置为它们的系统默认类型。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL计为收入]</td> 
      <td><p>如果您希望与此小时类型关联的小时条目影响您的收入计算，请选择此选项。</p>
      <p>病假和休假时间不能计为收入。</p>
      <p><b>注释</b></p>
      <p>当常规小时类型计为收入时，与记录时间的用户的配置文件关联的成本费率与小时成本关联。  
      </td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL 计为收入]**：如果您希望与此小时类型关联的小时条目影响您的收入计算，请选择此选项。

1. 单击&#x200B;**[!UICONTROL 创建小时类型]。**

## 停用小时类型

如果小时类型已过时，并且您不再希望用户将其小时条目与其关联，您可以停用小时类型。

停用小时类型会从[!DNL Workfront]中可见小时类型的任意位置隐藏小时类型。

要停用小时类型，请执行以下操作：

{{step-1-to-setup}}

1. 展开&#x200B;**[!UICONTROL 工时表与小时首选项]**，然后单击&#x200B;**[!UICONTROL 小时类型]**。

1. 选择要取消激活的小时类型。

1. 单击&#x200B;**[!UICONTROL 停用]**。
