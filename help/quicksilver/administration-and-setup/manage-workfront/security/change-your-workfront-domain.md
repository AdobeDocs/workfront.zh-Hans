---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: 更改Adobe Workfront域
description: 作为Adobe Workfront管理员和经授权的Workfront支持联系人，您可以向Workfront支持团队请求帮助，以更改贵组织的Workfront域。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# 更改Adobe Workfront域

>[!IMPORTANT]
>
>本页中介绍的过程仅适用于尚未载入Admin Console的组织。 如果贵组织已载入Adobe Admin Console，则无法更改您的Workfront域。
>
>有关因贵组织是否已登记到Adobe Admin Console而不同的过程列表，请参阅[基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

作为Adobe Workfront管理员和经授权的Workfront支持联系人，您可以向Workfront支持团队请求帮助，以更改贵组织的Workfront域。

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
   <td>规划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 请求域更改

1. 开始在Experience League上创建支持工单。
1. 在&#x200B;**描述**&#x200B;框中，包含所需的新域，以及希望新域上线的时间范围。
1. 完成填写支持案例的框，然后单击&#x200B;**提交**。

您还可以致电Workfront支持，获取有关更改域的帮助。

## 如果您是SSO客户，请更新新域

如果您的公司使用SSO，则在更改Workfront域后需要执行以下步骤。

>[!NOTE]
>
>如果您组织的Workfront实例已启用Adobe IMS，则此项不可用。 如果需要更多信息，请咨询您的网络或IT管理员。

{{step-1-to-setup}}

1. 在左侧边栏中，单击&#x200B;**系统** > **客户信息**，并确保您的域在“客户信息”页面上已更新。

1. 在左侧边栏中，单击&#x200B;**系统** > **单点登录(SSO)**。

1. 单击&#x200B;**下载SAML 2.0元数据**。
1. 下载文件后，打开它并确保以下各项：

   1. **entityID**&#x200B;正在指向新域。
   1. **`<md:AssertionConsumerService>`**&#x200B;中的所有位置都指向新域。

1. 将下载的元数据文件提供给您的身份提供程序，以便他们能够在其终端进行更新。
1. 确保为您的组织使用的所有Workfront集成更新域。
