---
title: 授予用户完全管理权限
description: 您可以授予用户对Workfront的完全管理访问权限。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '1550'
ht-degree: 4%

---

# 授予用户完全管理权限

<!--Audited: 12/2024-->

>[!IMPORTANT]
>
>本页中介绍的过程仅适用于尚未载入Admin Console的组织。 如果贵组织已载入到Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
>
>有关在Adobe Admin Console中授予完全管理员访问权限的说明，请参阅[在Adobe Admin Console中管理用户](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md)。
>
>有关因贵组织是否已登记到Adobe Admin Console而不同的过程列表，请参阅[基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

作为Adobe Workfront管理员，您可以通过分配系统管理员访问级别来创建另一个Workfront管理员。 具有此访问级别的用户对Workfront中的所有内容（包括他们自己未创建的项目）具有完全管理访问权限。

>[!NOTE]
>
>这与使用访问级别授予用户对系统特定区域的管理访问权限不同。 有关更多信息，请参阅以下内容：
>
>* [授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Workfront管理员的访问权限与具有管理权限的计划用户的访问权限](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights)（本文中）
>

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>新增：标准</p>
   <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。 </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 向单个用户授予系统管理员的完全访问权限

{{step-1-to-users}}

1. 单击要向其授予管理员权限的用户名。
1. 单击用户名右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-icon.png)，然后单击&#x200B;**编辑**。

   此时会显示&#x200B;**编辑人员**&#x200B;框。
1. 单击左侧面板中的&#x200B;**访问**。
1. 在&#x200B;**访问级别**&#x200B;下拉列表中，选择&#x200B;**系统管理员**&#x200B;访问级别。

   根据系统中进行的更改，此访问级别的名称可能已更改。

1. 单击&#x200B;**保存更改。**

   用户现在在系统中具有完全系统管理员权限。

## Workfront管理员的访问权限与具有管理权限的计划用户的访问权限  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

以下两个表显示了具有Workfront系统管理员访问级别的用户的访问权限与具有某些管理权限的计划许可证用户的访问权限之间的区别。

Workfront管理员可以查看系统中的所有对象（无论对象是由谁创建的）、创建新对象，以及修改或删除现有对象。 用户拥有系统中所有对象的完全访问权限。

拥有计划许可证且可以在一个区域中编辑功能的用户拥有对该区域中功能的完全访问权限。

>[!NOTE]
>
>具有计划许可证且被指定为组管理员的用户可以执行某些允许Workfront管理员执行的操作。 他们只能对其管理的组、其子组以及这些组和子组中的用户执行这些操作。 有关详细信息，请参阅[组管理员](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)。

* [访问“设置”区域](#access-to-the-setup-area)
* [访问对象](#access-to-objects)

### 访问“设置”区域 {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>区域/对象</th> 
   <th>Workfront管理员 </th> 
   <th>具有Plan许可证和某些管理权限的用户</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>项目首选项：项目</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>项目首选项：任务和问题</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>项目首选项：状态</td> 
   <td>完全访问</td> 
   <td> <p>无访问权限</p> </td> 
  </tr> 
  <tr> 
   <td>项目首选项：优先级</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>项目首选项：严重程度</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>项目首选项：汇率</td> 
   <td>完全访问</td> 
   <td>完全访问</td> 
  </tr> 
  <tr> 
   <td>流程：审批</td> 
   <td> <p>完全访问</p> </td> 
   <td>完全访问</td> 
  </tr> 
  <tr> 
   <td>流程：里程碑路径</td> 
   <td>完全访问</td> 
   <td>完全访问</td> 
  </tr> 
  <tr> 
   <td>自定义表单</td> 
   <td>完全访问</td> 
   <td> <p>管理他们创建的自定义表单或与他们共享的自定义表单。</p> <p>将他们创建的自定义表单或与他们共享的自定义表单附加到他们具有管理权限或参与权限的对象。</p> </td> 
  </tr> 
  <tr> 
   <td>回收站：最近删除</td> 
   <td>完全访问</td> 
   <td> <p>作为组管理员的用户可以恢复分配给其管理的组的项目，以及与这些项目关联的任务、问题或文档。</p> </td> 
  </tr> 
  <tr> 
   <td>回收站：最近已恢复</td> 
   <td>完全访问</td> 
   <td>作为组管理员的用户可以查看他们最近恢复的项目。</td> 
  </tr> 
  <tr> 
   <td>职位角色</td> 
   <td>完全访问</td> 
   <td> <p>修改但不删除现有工作角色。</p> <p>添加新工作角色。</p> </td> 
  </tr> 
  <tr> 
   <td>团队</td> 
   <td>完全访问</td> 
   <td> <p>无权创建团队。</p> <p>在创建或编辑用户时将现有团队添加到用户。</p> </td> 
  </tr> 
  <tr> 
   <td>组</td> 
   <td>完全访问</td> 
   <td> <p>无权创建组。</p> <p>只有组管理员可以管理其管理的组的组成员资格、子组和组级别状态。 </p> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>完全访问</td> 
   <td>完全访问</td> 
  </tr> 
  <tr> 
   <td>登录身份</td> 
   <td>完全访问 </td> 
   <td> <p>如果在他们的访问级别上启用了组管理访问权限，并且他们被指定为组管理员，则他们能够以他们所管理的组中的用户及其子组的身份登录。 他们无法以系统管理员身份登录。<br>有关为用户启用组管理访问权限的详细信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>计划</td> 
   <td>完全访问</td> 
   <td> <p>无权编辑计划。</p> <p>在用户级别访问将现有计划添加到其他用户。 </p> </td> 
  </tr> 
  <tr> 
   <td>时间表和小时：时间表配置文件</td> 
   <td>完全访问</td> 
   <td> <p>在用户级别访问以将现有时间表配置文件分配给用户。</p> <p>作为组管理员的用户可以为他们管理的组及其子组创建时间表配置文件。 </p> </td> 
  </tr> 
  <tr> 
   <td>时间表和小时：小时类型</td> 
   <td>完全访问</td> 
   <td> <p>在用户级别访问以将小时类型分配给用户。</p> </td> 
  </tr> 
  <tr> 
   <td>时间表和小时数：首选项</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>电子邮件：通知：事件通知</td> 
   <td>全部激活/取消激活</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>电子邮件：通知：提醒通知</td> 
   <td>完全访问</td> 
   <td>完全访问</td> 
  </tr> 
  <tr> 
   <td>电子邮件：通知：电子邮件模板</td> 
   <td>完全访问</td> 
   <td> <p>无权编辑电子邮件模板。</p> <p>访问以将现有电子邮件模板添加到提醒通知。</p> </td> 
  </tr> 
  <tr> 
   <td>电子邮件：自动提醒</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>电子邮件：邀请</td> 
   <td>完全访问</td> 
   <td> <p>无权编辑电子邮件邀请。</p> <p>只能从“人员”选项卡访问向未注册用户重新发送电子邮件邀请。</p> </td> 
  </tr> 
  <tr> 
   <td>电子邮件：设置</td> 
   <td>完全访问</td> 
   <td> <p>无访问权限</p> </td> 
  </tr> 
  <tr> 
   <td>记分卡</td> 
   <td>完全访问</td> 
   <td> <p>完全访问</p> </td> 
  </tr> 
  <tr> 
   <td>费用类型</td> 
   <td>完全访问</td> 
   <td> <p>无访问权限</p> </td> 
  </tr> 
  <tr> 
   <td>风险类型</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>访问级别</td> 
   <td> <p>具有修改所有访问级别的完全访问权限。</p> <p>默认情况下，无法修改系统管理员和外部用户访问级别。</p> </td> 
   <td> <p>无权编辑访问级别。</p> <p>将访问级别分配给在用户级别低于或等于其访问级别的其他用户。</p> </td> 
  </tr> 
  <tr> 
   <td>界面：布局模板</td> 
   <td>完全访问</td> 
   <td> <p>在用户级别访问以将现有布局模板分配给其他用户。 </p> <p>指定为组管理员的用户可以为他们管理的组和子组创建布局模板。</p> </td> 
  </tr> 
  <tr> 
   <td>界面：更新信息源</td> 
   <td>完全访问</td> 
   <td> <p>无权修改更新源。</p> <p>在编辑自定义Forms时，访问可在更新源中添加要跟踪的字段。</p> </td> 
  </tr> 
  <tr> 
   <td>界面：筛选器</td> 
   <td>完全访问</td> 
   <td> <p>无权在“设置”区域中创建筛选器。</p> <p>在对象列表中创建新筛选条件的访问权限。</p> </td> 
  </tr> 
  <tr> 
   <td>界面：视图</td> 
   <td>完全访问</td> 
   <td> <p>无权在“设置”区域中创建视图。</p> <p>在对象列表中创建新视图的访问权限。</p> </td> 
  </tr> 
  <tr> 
   <td>界面：分组</td> 
   <td>完全访问</td> 
   <td> <p>无权在“设置”区域中创建分组。</p> <p>在对象列表中创建新分组的访问权限。</p> </td> 
  </tr> 
  <tr> 
   <td>接口：列表控件</td> 
   <td>完全访问</td> 
   <td> <p>无访问权限</p> </td> 
  </tr> 
  <tr> 
   <td>文档：云提供商</td> 
   <td>完全访问</td> 
   <td> <p>无权配置云提供程序。</p> <p>将云提供商与Workfront集成后，可从文档选项卡访问将文档链接到云提供商或从云提供商链接到文档。</p> </td> 
  </tr> 
  <tr> 
   <td>文档：元数据映射</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>文档：SharePoint集成</td> 
   <td>完全访问</td> 
   <td> <p>无权配置SharePoint集成。</p> <p>在配置SharePoint与SharePoint的集成后，有权从“文档”选项卡将文档链接到Workfront以及从链接文档。</p> </td> 
  </tr> 
  <tr> 
   <td>文档：自定义集成</td> 
   <td>完全访问</td> 
   <td> <p>无权配置自定义集成。</p> <p>第三方提供商与Workfront集成后，可从文档选项卡将文档链接到第三方提供商或从第三方提供商链接文档。</p> </td> 
  </tr> 
  <tr> 
   <td>系统：品牌</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>系统：客户信息</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>系统：单点登录(SSO)</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>系统：更新SSO的用户</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>系统： Kick-Starts</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>系统：诊断</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
  <tr> 
   <td>系统：首选项</td> 
   <td>完全访问</td> 
   <td>无访问权限</td> 
  </tr> 
 </tbody> 
</table>

### 访问对象 {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>区域/对象</th> 
   <th>Workfront管理员 </th> 
   <th>具有Plan许可证和某些管理权限的用户</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>日程表</td> 
   <td>完全访问</td> 
   <td>管理他们创建的日历以及与他们共享的日历。</td> 
  </tr> 
  <tr> 
   <td>仪表板</td> 
   <td>完全访问</td> 
   <td>管理他们创建的功能板以及与他们共享的功能板。</td> 
  </tr> 
  <tr> 
   <td>文档</td> 
   <td>完全访问</td> 
   <td>管理他们上传的文档或与他们共享的文档。</td> 
  </tr> 
  <tr> 
   <td>问题</td> 
   <td>完全访问</td> 
   <td>管理他们创建的问题或与他们共享的问题。</td> 
  </tr> 
  <tr> 
   <td>项目组合</td> 
   <td>完全访问</td> 
   <td>管理他们创建的项目组合或与其共享的项目组合。 </td> 
  </tr> 
  <tr> 
   <td>项目群</td> 
   <td>完全访问</td> 
   <td>管理他们创建的程序或与他们共享的程序。</td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td>完全访问</td> 
   <td>管理他们创建的项目或与他们共享的项目。</td> 
  </tr> 
  <tr> 
   <td>报告</td> 
   <td>完全访问</td> 
   <td>管理他们创建的报告或与他们共享的报告。 查看、复制和编辑系统报告。</td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td>完全访问</td> 
   <td>管理他们创建的任务或与共享的任务</td> 
  </tr> 
  <tr> 
   <td>模板</td> 
   <td>完全访问</td> 
   <td>管理他们创建的模板或与他们共享的模板</td> 
  </tr> 
  <tr> 
   <td>时间表</td> 
   <td>完全访问</td> 
   <td>完全访问</td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td>完全访问</td> 
   <td> <p>有限访问</p> <p>他们无法将组分配给不是组管理员的用户或非公共组。</p> <p>他们无法将访问级别分配给高于其自身访问级别的用户。</p> <p>如果在他们的访问级别上启用了组管理访问权限，并且他们被指定为组的组管理员，则他们可以重置密码并以其管理的组及其子组中的用户身份登录。 他们无法重置密码或以系统管理员身份登录。<br>有关为用户启用组管理访问权限的详细信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>
