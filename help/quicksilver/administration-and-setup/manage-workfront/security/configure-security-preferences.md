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
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/46D3BBajFk39FP-dMDk0SuSSGM5nYPKas11Bs159R9Y
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1e6380b0422efdd98449ab1e74cadb4f330917f1
workflow-type: tm+mt
source-wordcount: 1155
ht-degree: 8%

---

# 配置系统偏好设置

{{preview-fast-release-general}}

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

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td><p>“任一”</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p><p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

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
      <td role="rowheader">允许人员使用Workfront的移动应用程序</td> 
      <td> <p>允许用户访问移动设备应用程序（适用于iPad和移动设备应用程序的Workfront View）</p> <p>此选项默认处于启用状态。 </p> <p>有关Workfront视图的信息，请参阅<a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">使用Adobe Workfront视图</a>。 有关移动设备应用程序的详细信息，请参阅<a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">使用Adobe Workfront移动设备应用程序：文章索引</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>使用电子邮件地址与没有Workfront帐户的人员协作</p> </td> 
      <td>允许Workfront用户通过包含其电子邮件地址而非姓名与没有Workfront帐户的用户共享某些项目。用户可以使用其电子邮件地址与外部用户共享以下项目：
       <ul>
        <li>文档<br></li>
        <li>文档请求<br></li>
        <li>文档审批</li>
        <li>日程表</li>
       </ul><p>此选项默认处于启用状态。</p> <p><b>重要信息</b>：如果禁用此选项，则外部用户访问级别在Workfront实例中不可用。 有关详细信息，请参阅<a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">内置访问级别</a>。</p> </td> 
     </tr> 
     <!--
     <tr> 
      <td role="rowheader">Require external users to register with a password</td> 
      <td> <p>Requires external users to register before they are able to view items in Workfront. By default, this option is disabled. When you enable this option, people without a Workfront account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr>
     -->
     <tr> 
      <td role="rowheader">自定义帮助 URL</td> 
      <td>允许您定义主菜单帮助图标要转到的内部自定义帮助站点。 有关详细信息，请参阅<a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">配置自定义帮助URL</a>。</p></td> 
     </tr>
    <tr> 
      <td role="rowheader">在访问级别内禁用自动升级</td> 
      <td>您可以禁用参与者访问级别的自动升级过程。 选中此设置后，超过其批准决策限制的参与者许可证用户必须由管理员手动升级到新许可证。</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">启用优先级工作列表 </td> 
      <td>允许您选择为用户启用或禁用“优先级”工作列表体验。 用户仍然可以在Workfront中看到优先级图标，但是他们无权访问该功能。 有关优先级的详细信息，请参阅<a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">开始使用优先级</a>。</td> 
     </tr>
     <tr>
      <td><span class="preview">批量编辑时始终强制要求必需字段</span></td>
      <td><span class="preview"><p>允许您选择在批量编辑对象时是否强制用户在必填字段中输入信息。</p> <p>选择此选项时，必填字段必须具有值，才能以批量编辑模式保存。 如果必填字段至少缺少一个批量选定对象的值，则不允许保存。</p> <p>如果未选择此选项，则只有在用户修改必填字段时，才会强制执行该字段。 如果未修改字段，则会将其视为可选字段，且不会验证该字段。</p></span></td>
     </tr>
     <tr> 
      <td role="rowheader">存储偏好设置 </td> 
      <td>在此部分中，您可以启用Adobe Cloud首选项。允许您选择为整个组织或特定组启用或禁用Adobe云存储。 
      <p>更新以下信息：</p>
      <ul><li><b>默认值</b>：选择旧版Workfront存储或Adobe云存储</li>
      <li><b>允许用户选择存储提供程序</b>：这允许用户在创建Workfront对象时在这两种存储类型之间进行选择。</li>
      <li><b>应用于</b>：选择默认设置是应用于整个组织还是应用于特定组</li>
      <li><b>选择要转换为Adobe云存储的项目组合</b>：选择要自动从Workfront旧存储转换为Adobe云存储的项目组合。 保存系统首选项时，将转换项目组合。</li></ul>     
    有关Adobe云存储的详细信息，请参阅<a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md">为您的组织启用Adobe云存储</a>。</td></tr>
    <tr> 
      <td role="rowheader">选择要转换为Adobe云存储的项目组合 </td> 
      <td>允许您将现有的旧版Workfront存储产品组合转换为Adobe云存储。 有关详细信息，请参阅<a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md">将旧项目组合转换为Adobe云存储</a>。</td> 
     </tr>
     <tr> 
      <td role="rowheader">启用 AI </td> 
      <td>通过打开AI首选项区域中的设置，您可以启用AI，包括AI助手。 <p><b>注意</b>：您的组织必须满足特定要求才能启用AI。 有关AI的详细信息（包括要求），请参阅<a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md">AI助手概述</a>。</p></td> 
     </tr>
    <tr> 
      <td role="rowheader">AI 表格填写 </td> 
      <td>允许人员使用Form Fill with AI自动填写请求表单。 有关详细信息，请参阅<a href="/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md">使用由AI提供支持的表单填写，以使用提示或文档填写请求</a>。</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">在请求表单中自动完成智能 </td> 
      <td>允许您选择启用根据先前的请求数据自动完成请求表单的功能。 有关表单自动完成的更多信息，请参阅<a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md">从以前的数据中自动填写请求</a>。</td> 
     </tr>
    <tr> 
      <td role="rowheader">规划设计器</td> 
      <td>这仅适用于已购买Workfront Planning包的客户。 启用此设置可让您的用户使用Planning Designer创建和编辑工作区。 有关信息，请参阅<a href="/help/quicksilver/planning/general/planning-ai-designer.md">Adobe Workfront规划Designer入门</a>。</td> 
     </tr>
     <tr> 
      <td role="rowheader">选择加入 AI Beta </td> 
      <td>允许您选择启用Beta中的当前人工智能功能。 如果启用此选项，则可以选择要启用的AI Beta功能。 有关每个AI Beta功能的更多信息，请单击该功能旁边的信息图标。</td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">只读 MCP 工具</span></td> 
      <td><span class="preview">允许Workfront MCP服务器对Workfront数据执行读取操作 — 例如，查找或列出项目、任务或其他项目。 此选项默认处于启用状态。<p>有关Workfront MCP服务器的详细信息，请参阅<a href="/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md">配置Adobe Workfront MCP服务器</a>。</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">写入 MCP 工具</span></td> 
      <td><span class="preview">允许Workfront MCP服务器对Workfront数据执行创建、更新和删除操作。 默认禁用此选项。<p>有关Workfront MCP服务器的详细信息，请参阅<a href="/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md">配置Adobe Workfront MCP服务器</a>。</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader">测试环境</td> 
      <td>允许您访问Workfront测试环境。 有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">Adobe Workfront预览沙盒环境</a>。</p></td> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

   您在此处保存的更改会影响Workfront中所有用户的体验，以及作为外部用户与系统交互的任何用户的体验。
