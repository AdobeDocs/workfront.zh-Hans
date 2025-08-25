---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 配置系统首选项
description: 作为Adobe Workfront管理员，您可以为Workfront系统配置首选项，包括安全首选项。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 945fa710e98b094a37258d5c94f7b1a2eb056abb
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 5%

---

# 配置系统偏好设置

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

{{important-admin-console-onboard}}

作为Adobe Workfront管理员，您可以为Workfront系统配置首选项，包括：

* 从移动应用程序和其他集成应用程序访问Workfront
* 将Workfront嵌入到iframe的规则

您在系统首选项中所做的更改将影响您系统中的所有用户，以及他们在Workfront中的体验。

我们建议您在Workfront实施期间配置系统首选项，之后只需偶尔重新访问一次。

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
   <td><p>新增：标准</p>
   <p>或</p>
   <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 配置您的系统首选项

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**系统** > **首选项**。

1. 选择以下任一字段来建立组织的设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>启用快速发布过程</p> </td> 
      <td>允许您为组织启用每月的Workfront版本，而不是每季度的版本。</p><p>有关快速发布过程的详细信息，请参阅<a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">为您的组织启用或禁用快速发布</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>允许在iframe中嵌入Workfront</p> </td> 
      <td>允许在iframe中嵌入Workfront。<p>默认禁用此选项。</p><p><b>重要信息</b>：在iframe中显示基于Web的应用程序会使应用程序容易出现点击劫持安全漏洞。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">在 Office 365 加载项中允许进行 SAML 2.0 身份验证</td> 
      <td> <p>当Workfront与SAML 2.0单点登录解决方案集成时，允许您仅将Workfront嵌入到iframe中，以用于Office 365加载项。 </p> <p>此选项默认处于启用状态。</p> <p><b>注意</b>：如果启用上述选项<strong>允许在iframe中嵌入Workfront</strong>，则选项<strong>在Office 365加载项中允许SAML 2.0身份验证</strong>已启用并灰显。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">创建外部页面URL时启用会话信息</td> 
      <td> <p>允许用户在将外部页面添加到功能板时使用站点的会话ID信息。</p> <p>此选项不安全，默认情况下处于关闭状态。 建议改用OAuth进行集成。</p> <p>有关将外部页面添加到仪表板的详细信息，请参阅<a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">在仪表板中嵌入外部网页</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许人员使用Workfront的移动应用程序和Workfront Outlook加载项</td> 
      <td> <p>允许用户访问移动设备应用程序(适用于iPad和移动设备应用程序的Workfront View)和Workfront Outlook应用程序。</p> <p>此选项默认处于启用状态。 </p> <p>有关Workfront视图的信息，请参阅<a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">使用Adobe Workfront视图</a>。 有关移动设备应用程序的详细信息，请参阅<a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">使用Adobe Workfront移动设备应用程序：文章索引</a>。</p> <p>有关Outlook插件的详细信息，请参阅<a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">为Outlook设置Adobe Workfront</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>使用电子邮件地址与没有Workfront帐户的人员协作</p> </td> 
      <td>允许Workfront用户通过包含其电子邮件地址而非姓名与没有Workfront帐户的用户共享某些项目。 用户可以使用其电子邮件地址与外部用户共享以下项目：
       <ul>
        <li>文档<br></li>
        <li>文档请求<br></li>
        <li>文档审批</li>
        <li>日程表</li>
       </ul><p>此选项默认处于启用状态。</p> <p><b>重要信息</b>：如果禁用此选项，则外部用户访问级别在Workfront实例中不可用。 有关详细信息，请参阅<a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">内置访问级别</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">要求外部用户使用密码注册</td> 
      <td> <p>要求外部用户先注册，然后才能在Workfront中查看项目。 默认情况下，此选项处于禁用状态。 启用此选项后，对于没有Workfront帐户但通过电子邮件地址包括在某些更新中的用户，系统将提示他们先创建帐户，然后才能查看其所包含的项目。 这将为他们创建一个外部用户帐户。</p> <p>默认禁用此选项。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在以下时段后自动注销用户：</td> 
      <td> 可让您指定用户在一段时间不活动后退出Workfront的时间。 默认情况下，用户在8小时不活动后被注销。 <p>此选项还会影响使用单点登录解决方案的Workfront客户。</p> <p>此设置不适用于已迁移到Adobe IMS的组织。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">在以下时段后自动注销移动用户： </td> 
      <td>可让您指定用户在一段时间不活动后何时注销Workfront应用程序。 默认情况下，用户会在处于非活动状态7天后注销。 <p>此选项还会影响使用单点登录解决方案的Workfront客户。</p> <p>此设置不适用于已迁移到Adobe IMS的组织。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义帮助 URL</td> 
      <td>允许您定义主菜单帮助图标要转到的内部自定义帮助站点。 有关详细信息，请参阅<a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">配置自定义帮助URL</a>。</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">系统中的用户将默认看到新主页体验 </td> 
      <td>可让您指定默认情况下用户是否会看到新主页体验。 启用后，用户将默认看到新主页体验，但仍可以选择根据个人情况启用或禁用新主页。 禁用后，用户将不会看到允许他们切换到新主页的横幅，但是，他们仍然可以通过在实例URL末尾手动输入<code>/home/workspaces</code>来导航到他们的新主页。 默认情况下，此设置处于启用状态。</td> 
     </tr>
     <tr> 
      <td role="rowheader">启用优先级工作列表 </td> 
      <td>允许您选择为用户启用或禁用“优先级”工作列表体验。 用户仍然可以在Workfront中看到优先级图标，但是他们无权访问该功能。 有关优先级的详细信息，请参阅<a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">开始使用优先级</a>。</td> 
     </tr>
     <tr> 
      <td role="rowheader">测试环境</td> 
      <td>允许您访问Workfront测试环境。 有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">Adobe Workfront预览沙盒环境</a>。</p></td> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

   您在此处保存的更改会影响Workfront中所有用户的体验，以及作为外部用户与系统交互的任何用户的体验。
