---
title: 导出自定义表单和对象详细信息
description: 导出自定义表单和对象详细信息
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 1%

---

# 导出自定义表单和对象详细信息

<!--Audited: 10/2025-->

您可以将对象的“概述”和“自定义表单”信息从“详细信息”部分导出到PDF文件。 然后，您可以打印或与其他用户共享PDF。

以下对象支持此功能：

* 项目
* 任务
* 问题
* 组合
* 项目群

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>Workfront或组管理员使用布局模板删除的详细信息部分中的字段不显示。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront包</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront许可证</p> </td> 
   <td><p>对于问题：</p>
   <ul><li><p>参与者或更高版本</p></li>
   <li><p>申请人或以上</p> </li></ul>
   <p>对于项目和任务：</p>
   <ul><li><p>浅色或更高</p></li>
   <li><p>审阅者或更高版本</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看或更高版本的项目、任务和问题</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>对象权限</p> </td> 
   <td> <p>查看或授予您想要导出其表单的项目、任务或问题的更高权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Request or higher for issues</p> <p>Review or higher for projects and tasks</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Access level configurations*</strong> </td> 
   <td> <p>View or higher for Projects, Tasks, and Issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> <p>View or higher permissions to the project, task, or issue whose form you want to export</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 先决条件

在开始之前，您必须具备以下所有条件：

1. 为要从中导出该对象的特定对象创建自定义表单。
1. 将自定义表单附加到对象

   或

   具有附加自定义表单和编辑表单上信息的正确访问权限。

有关创建自定义表单的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

有关将表单附加到对象的信息，请参阅[将自定义表单添加到对象](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

## 导出详细信息部分中的信息

对于支持从对象的“详细信息”部分导出信息的所有对象，其导出信息都是相同的。

1. 转到您至少具有查看权限的项目、任务、项目组合、项目群或问题。
1. 单击左侧面板上的&#x200B;**“详细信息”项**，如&#x200B;**任务详细信息**。
1. （可选）如果未将自定义表单附加到对象，请在&#x200B;**添加自定义表单字段**&#x200B;中开始键入自定义表单的名称，然后当该表单出现在列表中时单击它。

   您最多可以添加10个表单。

1. （可选）更新详细信息部分中的信息，然后单击&#x200B;**保存更改**。
1. 单击右上角的&#x200B;**导出**&#x200B;下拉菜单，选择&#x200B;**概述**&#x200B;或要导出的表单，然后单击&#x200B;**导出**。

   如果要导出概述区域和所有自定义表单，您还可以选择&#x200B;**全选**。

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >可能存在以下情况：
   >
   >   * 当您的组或Workfront管理员取消选择概述区域中的所有字段并且对象附加了自定义表单时，概述部分不显示。
   >   * 当您的组或Workfront管理员取消选择概述区域中的所有字段，并且对象没有附加自定义表单时，导出下拉菜单不可见。
   >   * 当对象未附加自定义表单时，您只能导出概述区域。
   >   * 逻辑落后且在表单上不可见的自定义字段不导出。 有关将逻辑添加到自定义表单的信息，请参阅[将逻辑规则添加到自定义表单和字段](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)。

   将生成一个PDF文件并下载到您的计算机。 PDF文件包含以下信息：

   * 表单附加到的对象的名称
   * 导出PDF的用户的名称
   * 生成PDF的日期和时间
   * 您导出的表单的名称
   * 表单上填写的字段中的信息
