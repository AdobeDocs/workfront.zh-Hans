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
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 2%

---

# 配置系统的基本信息

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

在配置Adobe Workfront系统时，您可以在“客户信息”页面的“基本信息”部分管理有关贵组织的详细信息。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>新增：标准</p>
   或
   <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## 访问客户信息

客户代表贵组织的Workfront实例。 作为Workfront的客户，您具有此区域的独特选项。

要访问“客户信息”页面，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**系统** > **客户信息**。

   根据您购买的Workfront计划，“客户信息”页面中可能缺少某些部分。 如果您需要了解贵组织使用哪个Workfront计划，请联系您的客户代表。

   “客户信息”区域中提供的部分包括：

   * **基本信息**

     有关在Workfront中配置基本信息的信息，请参阅[配置基本信息](#configure-basic-info)。

   * **API密钥设置**

     有关API密钥设置的信息，请参阅[管理API密钥](../../administration-and-setup/manage-workfront/security/manage-api-keys.md)。

   * **IP 允许列表**

     有关将IP地址添加到用户可访问Workfront的允许列表的信息，请参阅[配置防火墙的允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

   * **许可证**

     有关许可证的信息，请参阅[管理系统中的可用许可证](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)。

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
      <td role="rowheader">区域设置</td> 
      <td>控制传出电子邮件中使用的语言、日期和数字格式。 创建新用户时，此处选择的区域设置是默认的。 用户可以在用户配置文件中修改其区域设置。 当用户修改其区域设置时，其来自Workfront的电子邮件中的语言、日期和数字格式与他们的配置文件首选项匹配。 有关修改配置文件首选项的详细信息，请参阅<a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">配置我的设置</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">存储配额</td> 
      <td> <p>这是Workfront实例中可用的文档存储空间量。<br>配额包含您直接上传到Workfront的文档。<br>它不包括：</p> 
       <ul> 
        <li>您从任何其他第三方服务提供商(SharePoint、Google Drive、Webdam、Box、Dropbox、任何其他文档资产管理提供商)链接到Workfront的文档。</li> 
        <li>您的Workfront数据（项目、任务、问题、用户等）。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">产品版本</td> 
      <td>这是分配给您的某种Workfront实例。 大多数Workfront客户的产品版本是<strong>企业</strong>。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。
