---
title: 授予用户完全管理访问权限
description: 您可以向用户授予对Workfront的完全管理访问权限。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 1%

---

# 授予用户完全管理访问权限

>[!IMPORTANT]
>
>此页面中描述的过程仅适用于尚未载入Admin Console的组织。 如果贵组织已载入Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
>
>有关在Adobe Admin Console中授予完全管理员访问权限的说明：
>
>* 请参阅 [在Workfront中使用Adobe Admin Console创建系统管理员](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create2)
>* 请参阅文章中的“编辑用户详细信息”部分 [单独管理用户](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) (在Adobe Admin Console文档中)。
>* 联系您的Adobe Admin Console管理员。
>
>有关根据贵组织是否已载入Adobe Admin Console而有所不同的步骤列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

作为Adobe Workfront管理员，您可以通过为其分配系统管理员访问级别来创建另一个Workfront管理员。 具有此访问级别的用户对Workfront中的所有内容（包括他们自己未创建的项目）具有完全的管理访问权限。

>[!NOTE]
>
>这与使用访问级别向用户授予对系统某些区域的管理访问权限不同。 有关更多信息，请参阅以下内容：
>
>* [授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Workfront管理员的访问权限与具有管理权限的计划用户的访问权限](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) 在本文中
>


## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。 有关更多信息，请参阅 <a href="#" class="MCXref xref selected">授予用户完全管理访问权限</a>.</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 向单个用户授予完全系统管理员访问权限

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **用户** ![](assets/users-icon-in-main-menu.png).

1. 单击要向其授予管理员权限的用户的名称。
1. 单击“更多”菜单 ![](assets/more-icon.png)，然后单击 **编辑**.

1. 在 **编辑人员** 框，单击 **访问**.

1. 在 **访问级别** 下拉列表中，选择 **系统管理员** 访问级别。

   根据系统中所做的更改，此访问级别的名称可能已发生更改。

1. 单击 **保存更改。**

   用户现在在系统中拥有完全的系统管理员权限。

## Workfront管理员的访问权限与具有管理权限的计划用户的访问权限  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

下表显示了具有Workfront管理员访问权限级别的用户与具有具有某些管理权限的计划许可证用户的访问权限之间的差异。

Workfront管理员可以查看系统中的所有对象（无论是谁创建的对象）、创建新对象以及修改或删除现有对象。 他们拥有对系统中所有对象的完全访问权限。

具有计划许可证且可以在一个区域中编辑功能的用户有权完全访问该区域的功能。

>[!NOTE]
>
>具有计划许可证且被指定为组管理员的用户可以执行Workfront管理员允许的某些操作。 他们只能为他们管理的组、其子组以及这些组和子组中的用户执行这些操作。 有关更多信息，请参阅 [组管理员](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [访问“设置”区域](#access-to-the-setup-area)
* [对对象的访问](#access-to-objects)

### 访问“设置”区域 {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>区域/对象</th> 
   <th>Workfront管理员 </th> 
   <th>具有计划许可证和某些管理权限的用户</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>项目首选项：项目</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>项目首选项：任务和问题</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>项目首选项：状态</td> 
   <td>完全访问</td> 
   <td> <p>无权访问</p> </td> 
  </tr> 
  <tr> 
   <td>项目首选项：优先事项</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>项目首选项：严重性</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>项目首选项：汇率</td> 
   <td>完全访问</td> 
   <td>完全访问</td> 
  </tr> 
  <tr> 
   <td>流程：批准</td> 
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
   <td>回收站：最近删除的</td> 
   <td>完全访问</td> 
   <td> <p>群组管理员用户可以恢复分配给他们管理的群组的项目，以及与这些项目关联的任务、问题或文档。</p> </td> 
  </tr> 
  <tr> 
   <td>回收站：最近已恢复</td> 
   <td>完全访问</td> 
   <td>群组管理员用户可以查看他们最近还原的项目。</td> 
  </tr> 
  <tr> 
   <td>职位角色</td> 
   <td>完全访问</td> 
   <td> <p>修改但不删除现有作业角色。</p> <p>添加新作业角色。</p> </td> 
  </tr> 
  <tr> 
   <td>团队</td> 
   <td>完全访问</td> 
   <td> <p>无权创建团队。</p> <p>在创建或编辑用户时，向用户添加现有团队。</p> </td> 
  </tr> 
  <tr> 
   <td>组</td> 
   <td>完全访问</td> 
   <td> <p>无权创建群组。</p> <p>只有组管理员才能管理其所管理组的组成员资格、子组和组级别状态。 </p> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>完全访问</td> 
   <td>完全访问</td> 
  </tr> 
  <tr> 
   <td>登录方式</td> 
   <td>完全访问 </td> 
   <td> <p>如果其组管理访问权限在其访问级别上启用，并且被指定为组管理员，则他们可以以其所管理组及其子组中用户的身份登录。 他们无法以系统管理员身份登录。<br>有关为用户启用组管理访问权限的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>计划</td> 
   <td>完全访问</td> 
   <td> <p>无权编辑计划。</p> <p>有权在用户级别向其他用户添加现有计划。 </p> </td> 
  </tr> 
  <tr> 
   <td>工时单和工时：时间表配置文件</td> 
   <td>完全访问</td> 
   <td> <p>有权在用户级别将现有时间表配置文件分配给用户。</p> <p>组管理员用户可以为其管理的组及其子组创建时间表配置文件。 </p> </td> 
  </tr> 
  <tr> 
   <td>工时单和工时：小时类型</td> 
   <td>完全访问</td> 
   <td> <p>有权在用户级别为用户分配小时类型。</p> </td> 
  </tr> 
  <tr> 
   <td>工时单和工时：首选项</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>电子邮件：通知：事件通知</td> 
   <td>激活/取消激活所有</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>电子邮件：通知：提醒通知</td> 
   <td>完全访问</td> 
   <td>完全访问</td> 
  </tr> 
  <tr> 
   <td>电子邮件：通知：电子邮件模板</td> 
   <td>完全访问</td> 
   <td> <p>无权编辑电子邮件模板。</p> <p>有权向提醒通知添加现有电子邮件模板。</p> </td> 
  </tr> 
  <tr> 
   <td>电子邮件：自动提醒</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>电子邮件：邀请</td> 
   <td>完全访问</td> 
   <td> <p>无权编辑电子邮件邀请。</p> <p>只能从“人员”选项卡中访问，以向未注册的用户重新发送电子邮件邀请。</p> </td> 
  </tr> 
  <tr> 
   <td>电子邮件：设置</td> 
   <td>完全访问</td> 
   <td> <p>无权访问</p> </td> 
  </tr> 
  <tr> 
   <td>记分卡</td> 
   <td>完全访问</td> 
   <td> <p>完全访问</p> </td> 
  </tr> 
  <tr> 
   <td>费用类型</td> 
   <td>完全访问</td> 
   <td> <p>无权访问</p> </td> 
  </tr> 
  <tr> 
   <td>风险类型</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>访问级别</td> 
   <td> <p>具有完全访问权限，可修改所有访问级别。</p> <p>默认情况下，无法修改系统管理员和外部用户访问级别。</p> </td> 
   <td> <p>无权编辑访问级别。</p> <p>将访问级别分配给用户级别中与其较低或相等的其他用户。</p> </td> 
  </tr> 
  <tr> 
   <td>界面：布局模板</td> 
   <td>完全访问</td> 
   <td> <p>有权在用户级别将现有布局模板分配给其他用户。 </p> <p>指定为群组管理员的用户可以为他们管理的群组和子群组创建布局模板。</p> </td> 
  </tr> 
  <tr> 
   <td>界面：更新信息源</td> 
   <td>完全访问</td> 
   <td> <p>无权修改更新馈送。</p> <p>编辑自定义Forms时，有权在更新信息源中添加要跟踪的字段。</p> </td> 
  </tr> 
  <tr> 
   <td>界面：过滤器</td> 
   <td>完全访问</td> 
   <td> <p>无权在“设置”区域中创建过滤器。</p> <p>有权在对象列表中创建新过滤器。</p> </td> 
  </tr> 
  <tr> 
   <td>界面：视图</td> 
   <td>完全访问</td> 
   <td> <p>无权在“设置”(Setup)区域中创建视图。</p> <p>有权在对象列表中创建新视图。</p> </td> 
  </tr> 
  <tr> 
   <td>界面：分组</td> 
   <td>完全访问</td> 
   <td> <p>无权在“设置”区域创建分组。</p> <p>有权在对象列表中创建新分组。</p> </td> 
  </tr> 
  <tr> 
   <td>界面：列表控件</td> 
   <td>完全访问</td> 
   <td> <p>无权访问</p> </td> 
  </tr> 
  <tr> 
   <td>文档：云提供商</td> 
   <td>完全访问</td> 
   <td> <p>无权配置云提供程序。</p> <p>在云提供商与Workfront集成之后，即可从“文档”选项卡中，访问与云提供商关联文档的权限。</p> </td> 
  </tr> 
  <tr> 
   <td>文档：元数据映射</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>文档：SharePoint集成</td> 
   <td>完全访问</td> 
   <td> <p>无权配置SharePoint集成。</p> <p>在配置了SharePoint与Workfront的集成后，可从“文档”选项卡访问将文档链接到SharePoint和从链接文档。</p> </td> 
  </tr> 
  <tr> 
   <td>文档：自定义集成</td> 
   <td>完全访问</td> 
   <td> <p>无权配置自定义集成。</p> <p>在第三方提供商与Workfront集成后，从“文档”选项卡访问与第三方提供商的链接文档和从第三方提供商链接文档。</p> </td> 
  </tr> 
  <tr> 
   <td>系统：品牌策略</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>系统：客户信息</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>系统：单点登录(SSO)</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>系统：更新SSO用户</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>系统：启动</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>系统：诊断</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
  <tr> 
   <td>系统：首选项</td> 
   <td>完全访问</td> 
   <td>无权访问</td> 
  </tr> 
 </tbody> 
</table>

### 对对象的访问 {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>区域/对象</th> 
   <th>Workfront管理员 </th> 
   <th>具有计划许可证和某些管理权限的用户</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>日历</td> 
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
   <td>管理他们创建的项目或与他们共享的项目。</td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td>完全访问</td> 
   <td>管理他们创建的项目或与他们共享的项目。</td> 
  </tr> 
  <tr> 
   <td>报告</td> 
   <td>完全访问</td> 
   <td>管理他们创建的报表或与他们共享的报表。 查看、复制和编辑系统报告。</td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td>完全访问</td> 
   <td>管理他们创建的任务或与共享的任务</td> 
  </tr> 
  <tr> 
   <td>模板</td> 
   <td>完全访问</td> 
   <td>管理用户创建的模板或与其共享的模板</td> 
  </tr> 
  <tr> 
   <td>时间表</td> 
   <td>完全访问</td> 
   <td>完全访问</td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td>完全访问</td> 
   <td> <p>有限访问</p> <p>他们不能将组分配给他们不是群组管理员的用户或非公共群组。</p> <p>他们无法为高于其自身访问级别的用户分配访问级别。</p> <p>如果其组管理访问权限在其访问级别上启用，并且在组上指定为组管理员，则他们可以重置的密码并以其所管理组及其子组中的用户身份登录。 他们无法重置的密码或以系统管理员身份登录。<br>有关为用户启用组管理访问权限的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
