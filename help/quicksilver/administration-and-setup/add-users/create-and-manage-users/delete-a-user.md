---
title: 删除用户
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 当用户离开您的组织时，可以从Workfront中删除该用户，不过我们建议取消激活用户，而不是删除他们。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# 删除用户

当用户离开您的组织时，您可以从Adobe Workfront中删除该用户。

>[!IMPORTANT]
>
>* 从系统中删除用户也会删除与您可能想要保留的用户相关联的信息。 我们建议取消激活用户，而不是删除用户。 有关更多信息，请参阅 [停用或重新激活用户](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
>* 此页面中描述的过程仅适用于尚未载入Admin Console的组织。 如果贵组织已载入Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
>
>从 [!DNL Adobe Admin Console] 停用 [!DNL Workfront]，但不会从中删除它们 [!DNL Workfront].
>
>  有关在Adobe Admin Console中删除用户的说明，请参阅文章中的“永久删除用户”部分 [单独管理用户](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 或联系Adobe Admin Console管理员。
>
>  有关根据贵组织是否已载入Adobe Admin Console而有所不同的步骤列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

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
   <td> <p>您必须具有以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 有关信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>. </p> </li> 
     <li> <p><b>用户</b> 在配置为 <b>编辑</b> 访问，使用 <b>创建</b> 至少两个中的一个 <b>用户管理员</b> 在 <b>优化设置</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>在这两个选项中，如果用户 <b>管理员（群组用户）</b> 启用后，您必须是用户所属的组的组管理员。</p> <p>有关 <b>用户</b> 在访问级别中设置，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 删除和停用用户

取消激活用户会导致发生以下情况：

* 如果Workfront校样组件与您的Workfront帐户相关联，则删除用户对Workfront和Workfront校样的许可证。 有关Workfront校样的更多信息，请参阅 [Workfront校样](../../../workfront-proof/workfront-proof.md).
* 不能再为用户分配工作。
* 无法再将用户添加到更新中。
* 无法再将用户添加到团队或群组。
* 无法再与用户共享对象。
* 它们与以下对象的关联保持不变：

   * 任务、问题、项目、项目组合
   * 仪表板

      >[!NOTE]
      >
      >如果您停用用户，并且无法再查看与用户关联的报表或功能板，则可能需要更新 **使用以下访问权限运行此报表：** 字段。\
      >要了解更多信息，请参阅 [为什么我无法访问已停用用户拥有的报表？](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) 部分 [报表常见问题解答](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) 文章。

   * 文档
   * 更新
   * 小时

* 如果用户已签出文档，则在您停用这些文档时，这些文档仍保持签出状态。 只有Workfront管理员才能重新签入。 有关签出文档的更多信息，请参阅 [签出文档](../../../documents/managing-documents/check-out-documents.md).

删除用户会导致发生以下情况：

* 如果Workfront校样组件与您的Workfront帐户关联，则删除用户对Workfront和Workfront校样的许可证。 有关Workfront校样的更多信息，请参阅 [Workfront校样](../../../workfront-proof/workfront-proof.md).
* 不能再为用户分配工作。
* 无法再将用户添加到更新中。
* 无法再将用户添加到团队或群组。
* 无法再与用户共享对象。
* 删除该用户与以下对象的关联：

   * 任务、问题、项目、项目组合
   * 仪表板

      >[!NOTE]
      >
      >此外，您还无法访问包含与已删除用户关联的功能板的自定义部分。\
      >要了解更多信息，请参阅 [如何访问包含已删除用户拥有的报表的功能板？](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) 部分 [报表常见问题解答](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) 文章。

   * 更新
   * 小时

      >[!NOTE]
      >
      >这些对象仍保留在Workfront中，但对象的所有者现在为空。

* 如果用户在“全局导航栏”的“文档”区域下上传了任何文档，则文档也会被删除。
* 如果用户签出了他们拥有的文档，并且文档在主“文档”区域（从“主菜单”访问）中上传，则这些文档将随用户一起删除。 有关签出文档的更多信息，请参阅 [签出文档](../../../documents/managing-documents/check-out-documents.md).

有关取消激活用户的更多信息，请参阅 [停用或重新激活用户](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

您可以一次永久删除一个用户，也可以同时永久删除多个用户。 删除个人用户时，必须等待删除过程完成，然后才能转到Workfront中的其他活动。 同时删除多个用户的过程将作为后台进程运行，这样在删除用户时，您就可以继续使用Workfront。

## 删除一个或多个用户

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **用户**.
1. 至少选择一个要删除的用户，单击“更多”菜单 ![](assets/more-icon.png)，然后单击 **删除**.
1. 在显示的框中，单击 **删除** 以确认删除。

   删除用户的过程将作为后台过程运行，以便您可以继续使用Workfront作为删除用户。

   根据您删除的用户数，该过程可能需要几分钟甚至几小时。

   在Workfront中收到用户被删除的确认函后，您可能会继续在系统中看到这些用户，直到在后台完成删除过程为止。

   以后，如果您发现一个或多个用户未成功删除，请尝试一次删除一个。
