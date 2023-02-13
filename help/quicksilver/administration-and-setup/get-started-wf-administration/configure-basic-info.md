---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 配置系统的基本信息
description: 在配置Adobe Workfront系统时，您可以在客户信息页面的基本信息部分中管理有关您组织的详细信息。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 2%

---

# 配置系统的基本信息

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

在配置Adobe Workfront系统时，您可以在客户信息页面的基本信息部分中管理有关您组织的详细信息。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> <col> 
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
   <td> <p>您必须是Workfront管理员。 有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 访问客户信息

客户表示贵组织的Workfront实例。 作为Workfront的客户，您在此区域拥有独有的选项。

要访问“客户信息”页面，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **系统** > **客户信息**.

   根据您购买的Workfront计划，“客户信息”页面中可能缺少某些部分。 如果您需要了解贵组织使用的Workfront计划，请联系您的客户代表。

   “客户信息”区域中提供的部分包括：

   * **基本信息**

      有关在Workfront中配置基本信息的信息，请参阅 [配置基本信息](#configure-basic-info).

   * **API 密钥设置**

      有关API密钥设置的信息，请参阅 [管理API密钥](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **IP 允许列表**

      有关将IP地址添加到用户可允许列表以访问Workfront的的信息，请参阅 [配置防火墙的允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * **许可证**

      有关许可证的信息，请参阅 [管理系统中的可用许可证](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

## 配置基本信息 {#configure-basic-info}

在“客户信息”页面的“基本信息”区域中，有关客户的某些详细信息由Workfront配置，并以只读模式显示。 您还可以配置其他详细信息。 您可以在此区域中编辑的任何选项都会对Workfront中的所有用户产生全局影响。

要在“客户信息”区域配置“基本信息”部分，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **系统** > **客户信息**.

1. 在 **基本信息** 的 **客户信息** 页面，找到有关您使用Workfront的实例的以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td>您的组织的名称，也与您公司的名称匹配。 该内容由Workfront添加，无法编辑。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">群集设置 </td> 
      <td>实例的群集编号。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理员电子邮箱</td> 
      <td> <p>您的Workfront管理员的电子邮件地址。 您可以编辑此字段以匹配您的某个Workfront管理员的电子邮件地址。 与此电子邮件地址关联的用户被视为您的Workfront系统的主要Workfront管理员。 来自Workfront的任何站点范围通信都会定向到此电子邮件地址，因此务必要保持其更新。</p> <p><b>注意</b>:您无法停用、删除或更改与管理员电子邮件关联的用户的访问级别。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">域</td> 
      <td> <p>域由Workfront在创建帐户时设置。</p> <p>该域可在用于访问Workfront的URL中标识您的唯一子域。<p>例如，如果您的组织已被分配域“mycompany”，则用于访问Workfront的URL为 <i>https://mycompany.my.workfront.com。</i></p><p>您无法自行编辑域。 如果要更改域，请联系Workfront客户支持。 有关联系Workfront客户支持的更多信息，请参阅 <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">联系客户支持</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">时区</td> 
      <td> <p>这是您的Workfront实例的默认时区。 您可以编辑此字段以匹配主Workfront位置的时区。 您选择的时区确定了以下内容： </p> 
       <ul> 
        <li>外发电子邮件中显示的日期和时间</li> 
        <li>新用户创建时的默认时区</li> 
       </ul> <p>用户可以在其配置文件下修改其Workfront实例的时区。 当用户修改其时区时，从Workfront发送的电子邮件中的日期和时间与其配置文件首选项匹配。 有关修改用户配置文件首选项的更多信息，请参阅 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">配置我的设置</a>. 创建新计划时，将选择该时区作为默认时区。 有关创建计划的详细信息，请参阅 <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">创建计划</a>.</p> <p>有关使用计划帮助用户跨时区在Workfront进行协作的信息，请参阅 <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">跨时区工作</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">地区</td> 
      <td>控制外发电子邮件中使用的语言、日期和数字格式。 创建新用户时，默认使用此处选择的区域设置。 用户可以在其用户配置文件中修改其区域设置。 当用户修改其区域设置时，从Workfront发送的电子邮件中的语言、日期和编号格式与其配置文件首选项相匹配。 有关修改配置文件首选项的更多信息，请参阅 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">配置我的设置</a>.</td> 
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
      <td>这是分配给您的Workfront实例类型。 大多数Workfront客户的产品版本是 <strong>企业</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。
