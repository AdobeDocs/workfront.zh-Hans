---
title: 删除用户
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 当用户离开您的组织时，可以从Workfront中删除该用户，但我们建议停用而不是删除这些用户。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 58567104d88e7e1363d4196aec8a36ee0566b95a
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 1%

---

# 删除用户

>[!IMPORTANT]
>
>本页中介绍的过程仅适用于尚未载入Adobe Business Platform的组织。 如果您已登记到Adobe Business Platform，则必须删除Adobe Admin Console中的用户。
>
>有关因贵组织是否已登记到Adobe业务平台而不同的过程列表，请参阅[基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

当用户离开您的组织时，您可以从Adobe Workfront中删除该用户。

>[!IMPORTANT]
>
>从系统中删除用户也会删除与您可能希望保留的用户相关联的信息。 我们建议停用而不是删除用户。 有关详细信息，请参阅[停用或重新激活用户](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/cn/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

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
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p><p>或</p><p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须具备以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 </li> 
     <li> <p>访问级别中的<b>用户</b>设置配置为<b>编辑</b>访问，其中<b>创建</b>以及<b>微调设置</b> <b>下至少启用</b>用户管理员<img src="assets/gear-icon-in-access-levels.png">选项之一。 </p> <p>在这两个选项中，如果启用了<b>用户管理员（组用户）</b>，您必须是该用户所属组的组管理员。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 删除与停用用户

停用用户会导致发生以下情况：

* 如果Workfront组件与您的Workfront Proof帐户关联，则删除用户对Workfront Proof和Workfront的许可证。 有关Workfront Proof的详细信息，请参阅[Workfront Proof：文章索引](../../../workfront-proof/workfront-proof.md)。
* 不能再为用户分配工作。
* 无法再将该用户添加到更新。
* 无法再向团队或组中添加用户。
* 无法再与用户共享对象。
* 它们与以下对象的关联保持不变：

   * 任务、问题、项目、项目组合
   * 仪表板

     >[!NOTE]
     >
     >如果您停用用户并且无法再查看与用户相关的报告或仪表板，则可能需要更新&#x200B;**使用**&#x200B;的访问权限运行此报告。\
     >要了解更多信息，请参阅[为什么无法访问已停用用户所拥有的报告？](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why)报告常见问题解答[文章的](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md)部分。

   * 文档
   * 更新
   * 小时

* 如果用户已签出文档，则当您取消激活这些文档时，它们仍保持签出状态。 只有Workfront管理员才能重新签入这些帐户。 有关签出文档的更多信息，请参阅[签出文档](../../../documents/managing-documents/check-out-documents.md)。

删除用户会导致发生以下情况：

* 如果Workfront组件与您的Workfront Proof帐户关联，请删除用户对Workfront Proof和Workfront的许可证。 有关Workfront Proof的详细信息，请参阅[Workfront Proof：文章索引](../../../workfront-proof/workfront-proof.md)。
* 不能再为用户分配工作。
* 无法再将该用户添加到更新。
* 无法再向团队或组中添加用户。
* 无法再与用户共享对象。
* 删除该用户与以下对象的关联：

   * 任务、问题、项目、项目组合
   * 仪表板

  <!--
     >[!NOTE]
     >
     >You also lose access to custom sections that contained dashboards associated to the deleted user.  
     >To learn more, see the [How do I access a dashboard that contains a report owned by a deleted user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.
     -->

   * 更新
   * 小时

     >[!NOTE]
     >
     >这些对象仍保留在Workfront中，但对象的所有者现在为空。

* 如果用户在“全局导航栏”的“文档”区域下上载了任何文档，则也会删除这些文档。
* 如果用户已签出他们拥有的文档，并且文档上载到主文档区域（从主菜单访问），则文档将随用户一起删除。 有关签出文档的更多信息，请参阅[签出文档](../../../documents/managing-documents/check-out-documents.md)。

有关停用用户的详细信息，请参阅[停用或重新激活用户](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。

您可以一次永久删除一个用户，也可以同时永久删除多个用户。 在删除单个用户时，您必须等待删除过程完成后再转到Workfront中的其他活动。 同时删除多个用户的过程将作为后台进程运行，因此您可以在删除用户后继续使用Workfront。

## 删除一个或多个用户

{{step-1-to-users}}

1. 至少选择一个要删除的用户，单击“更多”菜单![更多图标](assets/more-icon.png)，然后单击&#x200B;**删除**。
1. 在出现的框中，单击&#x200B;**删除**&#x200B;以确认删除。

   删除用户的过程将作为后台进程运行，因此您可以在删除一个或多个用户后继续使用Workfront。

   根据要删除的用户数，此过程可能需要几分钟甚至几小时。

   在Workfront中收到用户已被删除的确认后，您可以继续在系统中看到这些用户，直到在后台完成删除过程为止。

   稍后，如果您发现一个或多个用户未被成功删除，请尝试一次删除一个。
