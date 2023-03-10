---
title: 共享自定义表单
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以配置自定义表单的访问权限，以控制谁可以查看、共享和编辑该表单 — 人员、角色、组、团队、公司。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: f43a0aae33b96f5a061d9134122078d73fc21e40
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 1%

---

# 共享自定义表单

您可以配置自定义表单的访问权限，以控制谁可以查看、共享和编辑该表单 — 人员、角色、组、团队、公司。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront计划*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>计划</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对自定义表单的管理访问权限</p> <p>有关Workfront管理员如何授予此访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">授予用户对特定区域的管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有哪些计划、许可证类型或访问级别配置，请与Workfront管理员联系。

## 访问自定义表单 {#access-to-custom-forms}

默认情况下，当您创建新的自定义表单并且有人将其附加到对象时，分配给该对象的任何用户都可以查看和填写表单。 这包括拥有请求许可证的用户和外部用户。

但是，对于尚未附加自定义表单的对象，用户（即使他们具有Planner访问级别）也无法从“自定义Forms”下拉菜单中附加它，除非满足以下条件之一：

* 有人将自定义表单与用户或其团队、工作角色、组或公司共享，并授予了至少查看权限（选中了“附加到自定义数据”）
* 用户拥有计划许可证，其访问级别允许对自定义表单的管理访问权限

## 共享自定义表单

而不是将自定义表单保留在默认共享状态(在中介绍 [访问自定义表单](#access-to-custom-forms) 在本篇文章中)，您可以为特定用户、工作角色、组、团队和公司配置对表单的特定访问级别。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **自定义Forms**.
1. 选择自定义表单，然后单击 **共享**.
1. 在显示的框中，在下 **将自定义表单访问权限授予**，开始键入要与其共享自定义表单的用户、团队、工作角色、组或公司的名称，然后按键 **输入** 名称时。
1. 要调整您刚刚添加的用户、团队、工作角色、组或公司的访问权限，请单击名称右侧的下拉菜单，然后配置以下任一可用选项及其任何高级设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">查看它</td> 
      <td> <p>能够查看和填写对象上的自定义表单。</p> <p><b>注意</b>：对于拥有工作、查看和请求许可证的用户，这是最高可用选项。</p> <p>单击 <strong>高级设置</strong> 以指定是否允许以下项：</p> 
       <ul> 
        <li><strong>附加到自定义数据</strong>：能够将自定义表单附加到其拥有管理访问权限的项目、任务和问题</li> 
        <li> <p><strong>共享</strong>：能够与系统中的其他人员共享自定义表单</p> <p>拥有工作、审阅或请求许可证的用户只能通过API或自定义表单报表共享自定义表单。 有关更多信息，请参阅。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理它</td> 
      <td> <p>仅适用于拥有计划许可证的用户。 </p> <p>除了能够将表单添加到他们有权编辑的对象之外，用户还可以完全编辑自定义表单，包括添加、编辑和删除字段。</p> <p>单击 <strong>高级设置</strong> 指定是否允许以下项：</p> 
       <ul> 
        <li> <p><strong>附加到自定义数据</strong>：能够将自定义表单附加到其拥有管理访问权限的项目、任务和问题</p> </li> 
        <li><strong>删除</strong>：从系统中删除自定义表单</li> 
        <li><strong>共享</strong>：与系统中的其他人员共享自定义表单</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）重复步骤4 - 5以向列表中添加其他名称并配置其选项。
1. （可选）如果要将自定义表单（在其附加的对象上）的访问权限限制为以前步骤中指定的那些表单，请单击齿轮图标 ![](assets/gear-icon-settings-with-dn-arrow.jpg) 单击共享框右上角的 **删除系统范围访问权限**.

   如果你改变主意，可以点击 **使其在系统范围内可见** （默认选项）。

   >[!NOTE]
   >
   >* 当您将自定义表单设置为在系统范围内可见时，您仅允许用户查看和填写分配给他们的对象，而不允许将自定义表单附加到其他对象。 您可以使用步骤5中所述的“附加到自定义数据”选项授予将自定义表单附加到对象的功能。
   >* 大多数组织都希望确保系统中的每个人都可以填写自定义表单，将其附加到他们处理的对象上，并在报表中查看其数据。 如果您的组织是这种情况，我们建议您使用&quot;**使其在系统范围内可见**.” 以这种方式配置该选项时，对话框中显示“系统范围可见”：

   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >如果您担心某个自定义表单，当该表单附加到某些对象时，用户可能会在该表单中输入敏感数据，从而限制共享这些数据 *对象* 与其限制对表单本身的访问，不如限制对表单的访问。

1. 单击&#x200B;**保存**。

## 删除对自定义表单的访问权限

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **自定义Forms**.
1. 选择自定义表单，然后单击 **共享**.
1. 在显示的框中，单击您不想再对表单具有特殊访问权限的用户、团队、角色、组或公司名称右侧的X。
1. （可选）对于要删除的其他名称，重复上一步至。
1. 单击&#x200B;**保存**。
