---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 配置系统的基本信息
description: 在配置Adobe Workfront系统时，您可以在“客户信息”页面的“基本信息”部分管理有关贵组织的详细信息。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
last-update: 2026-04-29T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: bf86ab1dd526e2e5f3ef95ce0d6dca7fb6ca6c30
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 4%

---

# 配置系统的基本信息

{{highlighted-preview}}

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

在配置Adobe Workfront系统时，您可以在“客户信息”页面的“基本信息”部分管理有关贵组织的详细信息。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront包</td> 
   <td><p>“任一”</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p> <p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>您必须是Workfront管理员。 </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 访问客户信息

客户代表贵组织的Workfront实例。 作为Workfront的客户，您具有此区域的独特选项。

要访问“客户信息”页面，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**系统** > **客户信息**。

   根据您购买的Workfront软件包，“客户信息”页面中可能缺少某些部分。 如果您需要了解贵组织使用哪个Workfront包，请联系您的客户代表。

   “客户信息”区域中提供的部分包括：

   | 部分 | 更多信息 |
   |---------|-----------------|
   | **基本信息** | 有关在Workfront中配置基本信息的信息，请参阅[配置基本信息](#configure-basic-info)。 |
   | <span class="preview">**存储概述**</span> | <span class="preview">有关检查文档存储使用量和配额的信息，请参阅[检查文档存储限制](../../documents/managing-documents/check-document-storage.md)。</span> |
   | **API密钥设置** | 有关API密钥设置的信息，请参阅[管理API密钥](../../administration-and-setup/manage-workfront/security/manage-api-keys.md)。 |
   | **IP 允许列表** | 有关将IP地址添加到用户可访问Workfront的允许列表的信息，请参阅[配置防火墙的允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。 |
   | **电子邮件允许列表** | 有关向允许列表添加电子邮件的信息，请参阅[配置电子邮件](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md)。 |

   <!--
   * **License**

     For information about licenses, see [Manage available licenses in your system](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
     -->

## 配置基本信息 {#configure-basic-info}

在“客户信息”页面的“基本信息”区域中，有关客户的某些详细信息由Workfront配置，并以只读模式显示。 其他详细信息可由您配置。 您可以在此区域中编辑的任何选项都会对Workfront中的所有用户产生全局影响。

要在客户信息区域中配置基本信息部分，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**系统** > **客户信息**。

1. 在&#x200B;**客户信息**&#x200B;页面顶部的&#x200B;**基本信息**&#x200B;部分中，查找有关您使用Workfront的实例的以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td>您的组织的名称，也匹配您的公司的名称。 此内容由Workfront添加，无法编辑。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">群集设置 </td> 
      <td>实例的群集编号。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理员电子邮箱</td> 
      <td> <p>Workfront管理员的电子邮件地址。 您可以编辑此字段以匹配其中一个Workfront管理员的电子邮件地址。 与此电子邮件地址关联的用户被视为您的Workfront系统的主要Workfront管理员。 来自Workfront的任何站点范围通信都会定向到此电子邮件地址，因此保持其最新状态很重要。</p> <p><b>注意</b>：您无法停用、删除或更改与管理员电子邮件关联的用户的访问级别。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">域</td> 
      <td> <p>域在创建帐户时由Workfront设置。</p> <p>该域标识您用于访问Workfront的URL的唯一子域。<p>例如，如果贵组织已被分配域“mycompany”，则用于访问Workfront的URL为<i>https://mycompany.my.workfront.com。</i></p><p>您无法自己编辑域。 如果要更改域，请联系Workfront客户支持。 有关联系Workfront客户支持的详细信息，请参阅<a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">联系客户支持</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">时区</td> 
      <td> <p>这是Workfront实例的默认时区。 您可以编辑此字段以匹配主要Workfront位置的时区。 您所选择的时区决定了以下内容： </p> 
       <ul> 
        <li>在传出电子邮件中显示的日期和时间</li> 
        <li>新用户在创建时的默认时区</li> 
       </ul> <p>用户可以在个人资料下修改其Workfront实例的时区。 当用户修改其时区时，他们来自Workfront的电子邮件中的日期和时间与他们的配置文件首选项相匹配。 有关修改用户配置文件首选项的详细信息，请参阅<a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">配置我的设置</a>。 创建新计划时，该时区被选为默认时区。 有关创建计划的详细信息，请参阅<a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">创建计划</a>。</p> <p>有关使用计划帮助用户在Workfront中跨时区进行协作的信息，请参阅<a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">跨时区工作</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">默认电子邮件区域设置</td> 
      <td>控制传出电子邮件中使用的语言、日期和数字格式。 创建新用户时，此处选择的区域设置是默认的。 用户可以在用户配置文件中修改其区域设置。 当用户修改其区域设置时，其来自Workfront的电子邮件中的语言、日期和数字格式与他们的配置文件首选项匹配。 有关修改配置文件首选项的详细信息，请参阅<a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">配置我的设置</a>。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。
