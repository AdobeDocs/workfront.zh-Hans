---
title: 导出自定义表单和对象详细信息
description: 导出自定义表单和对象详细信息
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 1670edf153e57152e51adcfbda052eb74541d931
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 1%

---

# 导出自定义表单和对象详细信息

您可以将对象的“详细信息”部分中的“概述”和自定义表单信息导出到PDF文件。 然后，您可以打印该PDF或将其与其他用户共享。

以下对象支持此功能：

* 项目
* 任务
* 问题
* 项目组合
* 项目群

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>Workfront或组管理员使用布局模板删除的“详细信息”部分中的字段不显示。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront计划*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront许可证*</p> </td> 
   <td> <p>请求或更高级别的问题</p> <p>对项目和任务进行审核或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>访问级别配置*</strong> </td> 
   <td> <p>查看项目、任务和问题的视图或更高视图</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>对象权限</p> </td> 
   <td> <p>查看或更高权限，访问要导出其表单的项目、任务或问题</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须具备以下所有条件：

1. 为要从中导出的特定对象创建自定义表单。
1. 将自定义表单附加到对象

   或

   具有正确的访问权限，可附加自定义表单并编辑表单上的信息。

有关创建自定义表单的信息，请参阅 [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

有关将表单附加到对象的信息，请参阅 [将自定义表单添加到对象](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 导出详细信息部分中的信息

从对象的“详细信息”(Details)部分导出信息对于支持该信息的所有对象都是相同的。

1. 转到您至少具有“查看”权限的项目、任务、项目组合、项目或问题。
1. 单击 **“详细信息”项目** ，例如 **任务详细信息**.
1. （可选）如果对象没有附加自定义表单，请在 **添加自定义表单字段**，然后在列表中显示时单击。

   您最多可以添加10个表单。

1. （可选）更新“详细信息”部分中的信息，然后单击 **保存更改**.
1. 单击 **导出** 下拉菜单中，选择 **概述**，或要导出的表单，然后单击 **导出**.

   您还可以选择 **全选** 如果要导出“概述”区域和所有自定义表单。

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >可能存在以下情况：
   >
   >   
   >   
   >   * 当您的组或Workfront管理员取消选择“概述”区域中的所有字段，并且该对象附加了自定义表单时，“概述”部分将不显示。
   >   * 当您的组或Workfront管理员取消选择“概述”区域中的所有字段，并且该对象没有附加自定义表单时，“导出”下拉菜单将不可见。
   >   * 当对象未附加自定义表单时，您只能导出“概述”区域。
   >   * 逻辑后面且在表单上不可见的自定义字段不会导出。 有关将逻辑添加到自定义表单的信息，请参阅 [向自定义表单添加显示逻辑和跳过逻辑](../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md).


   将生成PDF文件并将其下载到您的计算机。 PDF文件包含以下信息：

   * 表单所附加到的对象的名称
   * 导出PDF的用户名
   * 生成PDF的日期和时间
   * 导出的表单的名称
   * 表单上填写的字段中的信息
