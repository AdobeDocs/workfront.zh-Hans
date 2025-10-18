---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 管理小时类型
description: 您可以将小时类型与小时条目关联。 小时类型是用于定义小时条目的标签。 小时类型可以是常规时间，也可以是项目特定的时间。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1127'
ht-degree: 1%

---

# 管理小时类型

<!--Audited: 05/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

<!--<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div>-->

小时类型是用于定义小时条目的标签。 您可以将小时类型与小时条目关联。

小时类型分为两类：

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td><p>[!UICONTROL 标准版]</p>
       <p>[!UICONTROL 计划]</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>[!UICONTROL 系统管理员]</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 内置小时类型

Workfront附带一组内置小时类型。 这些小时类型无法编辑或隐藏。

[!DNL Workfront]附带的小时类型包括：

* **[!UICONTROL 病假时间]**：不能与项目、任务或问题的小时条目关联的常规小时类型。 病假时数不能计为收入。
* **[!UICONTROL 休假时间]**：不能与项目、任务或问题的小时条目关联的常规小时类型。 休假时间不能计为收入。
* **[!UICONTROL 常规开销]**：不能与项目、任务或问题的小时条目关联的常规小时类型。 它可以在您的项目计划流程中计为收入。
* **[!UICONTROL 项目时间]**：只能与项目小时条目关联的常规小时类型。
* **[!UICONTROL 任务时间]**：只能与任务的小时条目关联的常规小时类型。
* **[!UICONTROL 问题时间]**：只能与问题的小时条目关联的常规小时类型。

## 创建小时类型

作为[!DNL Workfront]管理员，您可以在系统和项目级别为组织创建小时类型。

在系统级别定义小时类型后，用户可以定义哪些小时类型可用于特定项目或特定用户。

有关详细信息，请参阅[定义小时类型和可用性](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

要创建小时类型，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**时间表和小时数**，然后单击&#x200B;**小时类型**。

1. 在&#x200B;**小时类型**&#x200B;部分中，单击&#x200B;**新建小时类型**。
1. 在&#x200B;**新小时类型**&#x200B;对话框中，指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名称]</td> 
      <td>输入易于在系统中识别的小时类型名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 描述]</td> 
      <td>添加对小时类型的描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 作用域]</td> 
      <td> <p>在<strong>范围</strong>下拉菜单中选择小时类型是常规小时类型还是特定于项目的小时类型。</p> <p>常规小时类型仅在时间表中可见，并且不能与项目、任务或问题相关联。</p> <p><b>重要</b></p><p> 如果您具有特定于&lbrack;！UICONTROL项目的自定义小时类型，并且您将其更改为[!UICONTROL 常规]，则所有现有的任务、问题和项目小时数都会设置为它们的系统默认类型。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 计为收入]</td> 
      <td><p>如果您希望与此小时类型关联的小时条目影响您的收入计算，请选择此选项。</p>
      <p>病假和休假时间不能计为收入。</p>
      <p><b>注释</b></p>
      <p>当常规小时类型计为收入时，与记录时间的用户的配置文件关联的成本费率与小时成本关联。  
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

   小时类型将会添加到您的Workfront系统中，并且默认情况下处于激活状态。

## 编辑小时类型

作为[!DNL Workfront]管理员，您可以在系统和项目级别编辑组织的小时类型。

>[!NOTE]
>
>* 您无法编辑内置小时类型。
>* 您无法批量编辑小时类型。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**时间表和小时数**，然后单击&#x200B;**小时类型**。

1. 单击小时类型名称或选择小时类型，然后单击列表顶部的&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。
1. 在&#x200B;**编辑小时类型**&#x200B;对话框中，指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名称]</td> 
      <td>输入易于在系统中识别的小时类型名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 描述]</td> 
      <td>添加对小时类型的描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 作用域]</td> 
      <td> <p>在<strong>范围</strong>下拉菜单中选择小时类型是常规小时类型还是特定于项目的小时类型。</p> <p>常规小时类型仅在时间表中可见，并且不能与项目、任务或问题相关联。</p> <p><b>重要</b></p> <p>如果您具有特定于&lbrack;！UICONTROL项目的自定义小时类型，并且您将其更改为[!UICONTROL 常规]，则所有现有的任务、问题和项目小时数都会设置为它们的系统默认类型。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 计为收入]</td> 
      <td><p>如果您希望与此小时类型关联的小时条目影响您的收入计算，请选择此选项。</p>
      <p>病假和休假时间不能计为收入。</p>
      <p><b>注释</b></p>
      <p>当常规小时类型计为收入时，与记录时间的用户的配置文件关联的成本费率与小时成本关联。  
      </td> 
     </tr> 
    </tbody> 
   </table>


1. 单击&#x200B;**保存**。

   将保存您的更改并编辑小时类型。

## 停用小时类型

如果您不再希望用户将其小时类型与其关联，则可以停用这些小时类型。 停用小时类型会从[!DNL Workfront]中显示小时类型的任意位置隐藏它们。

>[!NOTE]
>
>* 您无法停用内置小时类型。
>* 您可以批量停用小时类型。
>* 在停用项目特定的小时类型时，为该类型记录的所有时间会自动默认为项目特定的内置小时类型。 例如，为项目记录的时间默认为项目时间小时类型；为任务记录的时间默认为任务时间小时类型。
>* 停用常规小时类型时，记录时间会保留在时间表上，但用户将来无法再为该小时类型记录时间。



要停用小时类型，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 时间表和小时数]**，然后单击&#x200B;**[!UICONTROL 小时类型]**。

1. 选择要取消激活的小时类型。 您可以选择多个小时类型。

1. 单击&#x200B;**更多**，然后单击&#x200B;**停用**。

   ![激活和停用小时类型链接](assets/activate-and-deactivate-hour-type-links.png)

   小时类型已停用，用户在记录小时数时无法再找到它。

1. （可选）要重新激活小时类型，请在&#x200B;**小时类型**&#x200B;列表中选择该类型，然后单击&#x200B;**更多** > **激活**。

