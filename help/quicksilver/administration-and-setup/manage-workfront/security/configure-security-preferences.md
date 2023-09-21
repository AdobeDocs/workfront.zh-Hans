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
source-git-commit: b8416108a16d973435d070f8d2738fee585cc6d3
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 2%

---

# 配置系统首选项

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}

作为Adobe Workfront管理员，您可以为Workfront系统配置首选项：

* 从移动应用程序和其他集成应用程序访问Workfront
* 将Workfront嵌入到iframe的规则

您在系统首选项中所做的更改将影响您系统中的所有用户，以及他们在Workfront中的体验。

我们建议您在Workfront实施期间配置系统首选项，之后只需偶尔重新访问一次。

## 访问要求

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
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 配置您的系统首选项

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **系统** > **偏好设置**.

1. 选择以下任一字段来建立组织的设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>启用快速审查流程</p> </td> 
      <td>允许您为组织启用每月的Workfront版本，而不是每季度的版本。</p><p>有关快速发布过程的详细信息，请参见 <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">为您的组织启用或禁用快速发布</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>允许嵌入 <strong>Workfront</strong> 在iframe中</p> </td> 
      <td>允许在iframe中嵌入Workfront。<p>此选项默认处于禁用状态。</p><p><b>重要</b>：在iframe中显示基于Web的应用程序，会使该应用程序容易遭受点击劫持安全漏洞的攻击。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">在 Office 365 加载项中允许进行 SAML 2.0 身份验证</td> 
      <td> <p>当Workfront与SAML 2.0单点登录解决方案集成时，允许您仅将Workfront嵌入到iframe中，以用于Office 365加载项。 </p> <p>此选项默认处于启用状态。</p> <p><b>注意</b>：如果启用上述选项， <strong>允许在iframe中嵌入Workfront</strong>，选项 <strong>在Office 365加载项中允许进行SAML 2.0身份验证</strong> 已启用并灰显。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">创建外部页面URL时启用会话信息</td> 
      <td> <p>允许用户在将外部页面添加到功能板时使用站点的会话ID信息。</p> <p>有关将外部页面添加到功能板的详细信息，请参阅 <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">在功能板中嵌入外部网页</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">让人们使用Workfront的移动应用程序和 <strong>Workfront</strong> Outlook加载项</td> 
      <td> <p>允许用户访问移动设备应用程序(适用于iPad和移动设备应用程序的Workfront View)和Workfront Outlook应用程序。</p> <p>此选项默认处于启用状态。 </p> <p>有关Workfront视图的信息，请参阅 <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">使用Adobe Workfront视图</a>. 有关移动设备应用程序的更多信息，请参阅 <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">使用Adobe Workfront移动应用程序</a>.</p> <p>有关Outlook插件的详细信息，请参阅 <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">设置适用于Outlook的Adobe Workfront</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>使用电子邮件地址与没有Workfront帐户的人员协作</p> </td> 
      <td>允许Workfront用户通过包含其电子邮件地址而非姓名与没有Workfront帐户的用户共享某些项目。 用户可以使用其电子邮件地址与外部用户共享以下项目：
       <ul>
        <li>文档<br></li>
        <li>文档请求<br></li>
        <li>文档审批</li>
        <li>日历</li>
       </ul><p>此选项默认处于启用状态。</p> <p><b>重要</b>：如果禁用此选项，则外部用户访问级别在Workfront实例中不可用。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Workfront中的内置访问级别</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">要求外部用户使用密码注册</td> 
      <td> <p>要求外部用户先注册，然后才能在Workfront中查看项目。 默认情况下，此选项处于禁用状态。 启用此选项后，对于没有Workfront帐户但通过电子邮件地址包括在某些更新中的用户，系统将提示他们先创建帐户，然后才能查看其所包含的项目。 这将为他们创建一个外部用户帐户。</p> <p>此选项默认处于禁用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在以下时段后自动注销用户：</td> 
      <td> 可让您指定用户在一段时间不活动后退出Workfront的时间。 默认情况下，用户在8小时不活动后被注销。 <p>此选项还会影响使用单点登录解决方案的Workfront客户。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在以下时段后自动注销移动用户： </td> 
      <td>可让您指定用户在一段时间不活动后何时注销Workfront应用程序。 默认情况下，用户会在处于非活动状态7天后注销。 <p>此选项还会影响使用单点登录解决方案的Workfront客户。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">系统中的用户将默认看到新主页体验 </td> 
      <td>可让您指定默认情况下用户是否会看到新主页体验。 启用后，用户仍可以选择单独启用或禁用“新建主页”。 禁用后，用户将无法选择使用新主页。 此选项默认处于启用状态。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

   您在此处保存的更改会影响Workfront中所有用户的体验，以及以外部用户身份与他们交互的任何用户的体验。
