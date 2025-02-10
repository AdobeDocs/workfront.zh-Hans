---
title: 共享对象的财务权限
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: 在分配访问级别时，Adobe Workfront管理员可以向您授予查看或编辑财务数据的权限。 有关详细信息，请参阅授予对财务数据的访问权限。
author: Alina
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
source-git-commit: 3bd377ba2dec29bb956632cf3e9e3e33afe4305d
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# 共享对象的财务权限

{{highlighted-preview}}

在分配访问级别时，Adobe Workfront管理员可以向您授予查看或编辑财务数据的权限。 有关详细信息，请参阅[授予对财务数据的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

除了授予用户的访问级别之外，您还可以授予他们查看或管理您有权共享的特定项目、任务或问题的财务的权限。

有关每个访问级别中的用户可以如何处理财务数据的信息，请参阅[适用于每个对象类型的功能](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)一文中的[财务数据](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia)部分。

## 访问要求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial&nbsp;Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
要共享对象的财务数据信息，必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限的项目、任务、问题和财务数据</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看至少包含查看财务权限的项目、任务和问题的权限或更高</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 共享对象并授予财务权限

向对象授予财务权限时，请考虑以下事项：

* 您可以向项目、任务、问题、<span class="preview">和费率卡</span>授予财务权限。
* 权限可以继承：如果您拥有项目的“查看财务”权限，则您会自动继承项目上任务和问题的“查看财务”权限。

要授予对象的财务权限，请执行以下操作：

1. 转到要与他人共享的任务、项目或问题。
1. 在对象名称附近，单击“更多”菜单![](assets/more-icon.png)，然后单击&#x200B;**共享**。

1. 在&#x200B;**授予`<Object name>`对**&#x200B;的访问权限字段中，开始键入要与其共享对象的用户、团队、角色、组或公司的名称。

   >[!TIP]
   >
   >您只能与活动用户、团队、角色或公司共享对象。

1. 如果所选名称的右侧出现下拉菜单，请单击以下可用选项之一：

   * **查看它**
   * **Contribute加入其中**
   * **管理它**

     ![](assets/12.png)      ![](assets/13.png) ![](assets/14.png)

1. 在同一下拉菜单中，单击&#x200B;**高级设置**，然后执行以下操作之一：

   * 如果您在上一步中选择了三个选项之一，请确保已选择&#x200B;**查看财务**。
   * 如果您在上一步中选择了&#x200B;**管理财务**，请确保已选择&#x200B;**管理财务**。

1. 单击&#x200B;**保存**。

## 所有共享级别的财务权限

下表显示授予用户查看、Contribute或管理对象权限后获得的财务权限： 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>操作</strong> </th> 
   <th><strong>管理</strong> </th> 
   <th><strong>Contribute</strong> </th> 
   <th><strong>视图</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>管理开票记录</td> 
   <td>✓ {\f13 }</td> 
   <td> <p> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>管理/查看角色计费和成本率</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>管理/查看用户计费和成本率</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>查看财务状况</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> ✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td><span class="preview">管理费率卡</span></td> 
   <td>✓ {\f13 }</td> 
   <td> <p> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span class="preview">查看费率卡</span></td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> ✓ {\f13 }</td> 
  </tr>
  <tr> 
   <td>在资源计划工具中按成本查看信息</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>资源规划工具中的预算资源*</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>在资源计划工具中查看资源*</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> <p>✓ {\f13 }</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;需要额外的资源管理权限。

有关资源管理访问权限的信息，请参阅[授予对资源管理的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)。
