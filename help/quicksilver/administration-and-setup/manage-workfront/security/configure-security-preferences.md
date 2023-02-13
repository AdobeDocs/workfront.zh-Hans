---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 配置系统安全首选项
description: 作为Adobe Workfront管理员，您可以为Workfront系统配置安全首选项。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 04cf9d37c681398f5a0e2b9d7d45c0f8b93ab44b
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 3%

---

# 配置系统安全首选项

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}

作为Adobe Workfront管理员，您可以为Workfront系统配置安全首选项：

* 从移动应用程序和其他集成应用程序访问Workfront
* 在iFrame中嵌入Workfront的规则

您在系统首选项中所做的更改会影响系统中的所有用户，以及这些用户在Workfront中的体验。

我们建议您在Workfront实施期间配置系统安全首选项，并且只是偶尔在之后重新访问它们。

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
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 配置系统安全首选项

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **系统** > **首选项**.

1. 在 **安全性** 部分中，选择以下任意字段以为贵组织建立安全设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>允许嵌入 <strong>Workfront</strong> iframe中</p> </td> 
      <td>允许您在iFrame中嵌入Workfront。<p>默认情况下，此选项处于禁用状态。</p><p><b>重要信息</b>:在iFrame中显示基于Web的应用程序，使应用程序容易遭受点击顶升安全漏洞。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">在 Office 365 加载项中允许进行 SAML 2.0 身份验证</td> 
      <td> <p>在将Workfront与SAML 2.0单点登录解决方案集成后，允许您仅在Office 365加载项的iFrame中嵌入Workfront。 </p> <p>默认情况下，此选项处于启用状态。</p> <p><b>注意</b>:如果启用上述选项， <strong>允许在iFrame中嵌入Workfront</strong>，选项 <strong>在Office 365加载项中允许SAML 2.0身份验证</strong> 已启用且灰显。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在创建外部页面URL时启用会话信息的使用</td> 
      <td> <p>允许用户在向功能板添加外部页面时使用网站的会话ID信息。</p> <p>有关将外部页面添加到功能板的更多信息，请参阅 <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">在功能板中嵌入外部网页</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许用户使用Workfront的移动应用程序和 <strong>Workfront</strong> Outlook外接程序</td> 
      <td> <p>允许用户访问移动应用程序(适用于iPad和移动电话应用程序的Workfront视图)和Workfront Outlook应用程序。</p> <p>默认情况下，此选项处于启用状态。 </p> <p>有关Workfront视图的信息，请参阅 <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">使用Adobe Workfront视图</a>. 有关移动设备应用程序的更多信息，请参阅 <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">使用Adobe Workfront移动设备应用程序</a>.</p> <p>有关Outlook插件的详细信息，请参阅 <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">设置Adobe Workfront for Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>使用电子邮件地址与没有Workfront帐户的人员协作</p> </td> 
      <td>允许Workfront用户通过包含其电子邮件地址而不是姓名，与没有Workfront帐户的人员共享某些项目。 用户可以使用其电子邮件地址与外部用户共享以下项目：
       <ul>
        <li>文档<br></li>
        <li>文档请求<br></li>
        <li>文档批准</li>
        <li>日历</li>
       </ul><p>默认情况下，此选项处于启用状态。</p> <p><b>重要信息</b>:如果禁用了此选项，则Workfront实例中的外部用户访问级别将不可用。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Workfront中的内置访问级别</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">要求外部用户使用密码注册</td> 
      <td> <p>需要外部用户先进行注册，然后才能查看Workfront中的项目。 默认情况下，此选项处于禁用状态。 启用此选项后，没有Workfront帐户的人员（通过其电子邮件地址包含在某些更新中）将被提示创建帐户，然后才能查看其中包含的项目。 这会为其创建外部用户帐户。</p> <p>默认情况下，此选项处于禁用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在以下时段后自动注销用户：</td> 
      <td> 允许您指定用户在处于不活动状态一段时间后何时注销Workfront。 默认情况下，用户在处于不活动状态8小时后会被注销。 <p>此选项还会影响使用单点登录解决方案的Workfront客户。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在以下时段后自动注销移动用户： </td> 
      <td>允许您指定用户在处于不活动状态一段时间后何时注销Workfront应用程序。 默认情况下，用户在处于不活动状态7天后会被注销。 <p>此选项还会影响使用单点登录解决方案的Workfront客户。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

   您在此处保存的更改会影响Workfront中所有用户以及以外部用户身份与他们进行交互的任何人的体验。
