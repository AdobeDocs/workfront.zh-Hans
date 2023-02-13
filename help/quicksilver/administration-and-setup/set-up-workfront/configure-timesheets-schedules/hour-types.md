---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 管理小时类型
description: 您可以将小时类型与小时条目关联。 小时类型是用于定义小时条目的标签。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# 管理小时类型

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

您可以将小时类型与小时条目关联。 小时类型是用于定义小时条目的标签。

有两组小时类型：

* **项目特定的小时类型**:此时记录项目、任务和问题。 特定于项目的小时类型可以与 [!DNL Adobe Workfront] 您可以在其中记录项目、任务和问题的时间。

   登录时 [!DNL Workfront]，具体项目可用的小时类型取决于系统、项目和用户级别中设置的配置选项。

   始终提供以下特定于项目的默认小时类型：

   * 项目时间
   * 任务时间
   * 问题时间

   的 [!DNL Workfront] 管理员确定提供哪些项目特定的小时类型，如 [定义工时单的工时类型和可用性](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   >[!NOTE]
   >
   >如果您在 [!DNL Workfront] 系统中，系统中的每个项目必须至少启用一个特定于项目的小时类型。 您无法在系统级别启用项目特定的小时类型，并且在项目级别没有项目特定的小时类型。

* **一般小时类型**:一般小时数不能与项目、任务或问题关联，并且会直接记录到时间表中。 有关记录时间的更多信息，请参阅 [日志时间](../../../timesheets/create-and-manage-timesheets/log-time.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront]计划</td> 
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

## 内置小时类型

Workfront提供一组内置的小时类型。 这些小时类型无法编辑，也无法隐藏。

随附的小时类型 [!DNL Workfront] 为：

* **[!UICONTROL 病假]**:不能与项目、任务或问题上的小时条目关联的常规小时类型。
* **[!UICONTROL 假期时间]**:不能与项目、任务或问题上的小时条目关联的常规小时类型。
* **[!UICONTROL 一般开销]**:不能与项目、任务或问题上的小时条目关联的常规小时类型。 但是，它可以在项目规划过程中计为收入。
* **[!UICONTROL 项目时间]**:一般的小时类型，只能与项目上的小时条目关联。
* **[!UICONTROL 任务时间]**:一般小时类型，只能与任务上的小时条目关联。
* **[!UICONTROL 问题时间]**：一般小时类型，只能与问题上的小时条目关联。

## 创建小时类型

As a [!DNL Workfront] 管理员，您可以在系统级别和项目级别上为组织创建新的小时类型。 在系统和项目级别上创建小时类型后，用户可以定义哪些小时类型可用于特定项目和用户。 有关更多信息，请参阅 [定义工时单的工时类型和可用性](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

要创建新的小时类型，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe] Workfront，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 工时单和小时数]** > **[!UICONTROL 小时类型]**.

1. 单击 **[!UICONTROL 新建小时类型].**
1. 在 **[!UICONTROL 新建小时类型]** 表单：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL名称]</td> 
      <td>为新小时键入一个在系统中易于识别的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL描述]</td> 
      <td>为您的小时类型添加描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL范围]</td> 
      <td> <p>通过在下拉菜单中选择正确的范围，定义小时类型是常规小时类型还是项目特定的小时类型。</p> <p>一般小时类型仅在时间表中可见，并且不能与项目、任务或问题关联。</p> <p><b>重要信息</b>:如果您的自定义小时类型为[!UICONTROL项目特定]，则您将其更改为[!UICONTROL常规]，则所有现有的任务、问题和项目小时数都将设置为其系统默认类型。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL计为收入]</td> 
      <td>如果希望与此小时类型关联的小时条目影响收入计算，请选择此选项。</td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL 计为收入]**:如果希望与此小时类型关联的小时条目影响收入计算，请选择此选项。

1. 单击 **[!UICONTROL 创建小时类型].**

## 停用小时类型

如果小时类型过时，并且您不再希望用户将其小时条目与它们关联，则可以停用小时类型。

取消激活小时类型会隐藏中任意位置的小时类型 [!DNL Workfront] 其中显示小时类型。

要停用小时类型，请执行以下操作：

1. 单击 **[!UICONTROL 设置]** 在的右上角附近 [!DNL Adobe Workfront] 中。

1. 展开 **[!UICONTROL 工时单和工时首选项]**，然后单击 **[!UICONTROL 小时类型]**.

1. 选择要停用的小时类型。

1. 单击 **[!UICONTROL 停用]**.
