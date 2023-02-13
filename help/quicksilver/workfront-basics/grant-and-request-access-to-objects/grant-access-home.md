---
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
title: 授予对“主页”区域中对象的访问权限
description: 用户可以请求访问Adobe Workfront中的对象。 有关请求访问的更多信息，请参阅请求对象的访问。
author: Alina
feature: Get Started with Workfront
exl-id: e0a69ed5-57c3-47ac-bb7a-65495f93b3e3
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# 授予对“主页”区域中对象的访问权限

用户可以请求访问Adobe Workfront中的对象。 有关请求访问的更多信息，请参阅  [请求对对象的访问](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).

如果您是对象的所有者，则可以授予或拒绝对“主页”区域中项目的访问权限。

## 访问要求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to projects, tasks, issues, or documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, issues, or documents</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对项目、任务、问题或文档的访问权限或更高权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目、任务、问题或文档的权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 授予对“主页”区域中对象的访问权限

1. 单击 **主页** 图标 ![](assets/home-icon-30x29.png) 在Adobe Workfront的左上角。

   >[!NOTE]
   >
   >您的Workfront管理员可以对环境中的主页图标进行以下更改：
   >
   >* 将其替换为自定义的图像，以说明您的组织。 在这种情况下，图标将与本文中显示的不同。
   >* 将链接到该页面的页面替换为其他页面。 在这种情况下，单击 **主菜单** ![](assets/main-menu-icon.png) ，然后单击 **主页**.


1. 在 **工作列表**，选择要管理的访问请求。\
   ![Screen_Shot_2018-07-02_at_11.35.29_AM.png](assets/screen-shot-2018-07-02-at-11.35.29-am-350x242.png)

1. 单击右上角的授予访问按钮。\
   根据请求的访问类型，按钮名称会发生更改。 例如，如果请求者要求获取“查看”访问权限，则按钮会显示 **授予视图访问权限**.\
   ![Grant_Access_2.png](assets/grant-access-2-350x98.png)

1. （可选）要授予与请求不同的访问级别，请单击授予访问按钮旁边的箭头，然后选择新访问权限。\
   出现一条消息，确认已授予访问权限。\
   或\
   单击 **忽略** 拒绝访问。\
   出现一条消息，确认已忽略访问。

## 为请求配置电子邮件通知

您可以配置您是否收到访问请求的电子邮件通知。 您的Workfront管理员可以禁用此功能(如 [为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md))。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **首选项**，或滚动到首选项部分。
1. 在 **发送电子邮件时间** 下拉列表中，选择或取消选择 **有人请求我访问**，具体取决于您是否希望其他用户请求您访问时接收电子邮件通知。

1. 单击 **保存更改**.
