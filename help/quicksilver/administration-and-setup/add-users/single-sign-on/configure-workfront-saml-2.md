---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: 使用 SAML 2.0 配置 Adobe Workfront
description: 作为Adobe Workfront管理员，您可以配置Workfront Web和移动应用程序以与用于单点登录(SSO)的安全断言标记语言(SAML) 2.0解决方案集成。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: 22ae8b489c63ba6eea1472cf415f95e375a94773
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 8%

---

# 使用 SAML 2.0 配置 Adobe Workfront

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

<!-- Audited: 12/2023 -->



>[!IMPORTANT]
>
>本页中介绍的过程仅适用于尚未载入Adobe Admin Console的组织。
>
>要映射已载入到Adobe Admin Console的组织中的用户属性，请参阅映射用户属性一文中的[在Adobe中映射用户属性](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience)。

作为Adobe Workfront管理员，您可以配置Workfront Web和移动应用程序以与用于单点登录(SSO)的安全断言标记语言(SAML) 2.0解决方案集成。

在Workfront中配置SAML 2.0后，如以下部分所述，您可以维护配置，如在身份提供程序中[更新SAML 2.0元数据](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)中所述。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td><p>任何</p></td> 
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

## 启用使用SAML 2.0对Workfront的身份验证

{{step-1-to-setup}}

1. 单击&#x200B;**系统** > **单点登录(SSO)。**

1. 在&#x200B;**类型**&#x200B;下拉列表中，选择&#x200B;**SAML 2.0.**

1. 在显示的选项顶部附近，单击&#x200B;**下载SAML 2.0元数据**&#x200B;以在计算机上下载文件。

   SAML 2.0身份提供程序需要一个XML文件，其中包含在Workfront实例中生成的信息。 下载文件后，您必须访问SAML 2.0身份提供程序服务器，并在该服务器上传Workfront SAML 2.0元数据XML文件。

1. 在Workfront中指定以下信息：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">服务提供者标识 </td>
      <td> 已为您填充的此URL将Workfront标识给您的身份提供程序。 例如： <code>&lt;yourcompany&gt;.com/SAML2</code>。</td>
     </tr>
     <tr>
      <td role="rowheader">绑定类型</span> </td>
      <td> <p>选择IDP服务器支持用于发送身份验证信息的方法：</p>
       <ul>
       <li>POST</li>
       <li>重定向</li>
       </ul> </td>
     </tr>
     <tr>
      <td role="rowheader">填充身份标识提供程序元数据中的字段 </td> 
      <td>在SAML 2.0 Identity Provider解决方案中，导出服务提供程序元数据XML文件并将其保存到计算机上的临时位置。 选择<strong>选择文件</strong>，然后查找并选择保存的文件以将其添加到Workfront配置。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">登录入口URL</span> </td> 
      <td>输入贵组织的常用登录门户。 这是用户登录以访问Workfront和与SAML 2.0集成的所有其他应用程序的URL。</td> 
     </tr>
     <tr>
      <td role="rowheader">注销URL</span> </td> 
      <td> <p>输入IDP服务器的注销URL。 Workfront在注销Workfront之前会向此URL发送HTTP请求。 当Workfront会话关闭时，这将关闭用户在远程服务器上的会话。</p> <p><b>注意</b>：仅当您的用户配置文件中启用了<strong>仅允许SAML 2.0身份验证</strong>选项时，您才会被重定向到注销URL。</p> </td>
     </tr>
     <tr>
      <td role="rowheader">更改密码 URL </td> 
      <td> <p> 指定要重定向用户以更改其密码的URL。 </p> <p>由于使用SAML 2.0凭据访问Workfront，因此必须向用户重定向到一个他们可以在其中更改其SAML 2.0密码的页面，而不是通过Workfront完成此活动。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">安全哈希算法 </td> 
      <td> <p>选择IDP支持的安全哈希算法(SHA)：</p> 
       <ul> 
       <li>SHA-1</li> 
       <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自动预配用户</span> </td> 
      <td> <p>当具有目录用户名和密码的新用户尝试首次登录Workfront时，此选项会自动在系统中创建用户。</p> <p>要在Workfront中创建用户，必须在目录提供程序中将Workfront数据属性映射到以下用户数据属性：</p> 
       <ul> 
       <li>名</li> 
       <li>姓</li> 
       <li>电子邮件地址</li> 
       </ul> 
       <p>选中该复选框后，将显示以下选项：</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>从下拉列表中选择要映射的Workfront用户属性，然后在用户目录中指定相应的目录属性。</p> 
       <p><strong>Directory Attribute</strong>字段应包含成功测试SAML 2.0配置时保存的“用户属性”表中的目录属性名称。</p> 
       <p>您可以在<strong>默认值</strong>字段中设置默认Workfront值。 您还可以根据SAML 2.0身份提供程序的值设置规则。</p> 
       <p><b>警告</b>：每次用户登录系统时，Workfront都会尝试映射下列属性。 因此，我们不建议映射访问级别。 如果属性映射不正确，您可以轻松删除管理访问权限。 单击<strong>添加映射</strong>以添加其他规则。
       </p> 
       <p>您可以映射以下Workfront属性：</p> 
      <ul> 
      <li> <p>访问级别</p> </li> 
      <li> <p>地址</p> </li> 
      <li> <p>地址 2</p> </li> 
      <li> <p>计费/小时</p> </li> 
      <li> <p>城市</p> </li> 
      <li> <p>公司</p> </li> 
      <li> <p>成本/小时</p> </li> 
      <li> <p>电子邮件地址</p> </li> 
      <li> <p>扩展</p> </li> 
      <li> <p>名</p> </li> 
      <li> <p>主组</p> </li> 
      <li> <p>主团队</p> </li> 
      <li> <p>工作角色</p> </li> 
      <li> <p>姓</p> </li> 
      <li> <p>布局模板</p> </li> 
      <li> <p>管理员</p> </li> 
      <li> <p>手机</p> </li> 
      <li> <p>电话号码</p> </li> 
      <li> <p>邮政编码</p> </li> 
      <li> <p>计划</p> </li> 
      <li> <p>State</p> </li> 
      <li> <p>时间表配置文件</p> </li> 
      <li> <p>标题</p> </li> 
      </ul>
      <p>完成映射用户属性后，单击<strong>保存</strong>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">证书 </td> 
      <td> <p>上载有效的SSL证书，以确保身份验证服务与Workfront之间的安全连接。 对于OnDemand帐户，始终需要证书。 您可以从SAML 2.0系统管理员处获取此证书。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理豁免 </td> 
      <td> <p>允许Workfront管理员使用他们的Workfront登录信息访问Workfront。 如果未选择此选项，Workfront管理员必须使用他们的SAML 2.0用户名和密码。</p> 
      <p>Workfront首先会尝试为具有Workfront系统管理员访问权限级别的用户通过SAML 2.0登录Workfront。 如果SAML 2.0身份验证失败，Workfront会为Workfront管理员使用本地身份验证。</p> 
      <p>我们建议您始终选择此选项，以便在您的SAML 2.0提供商暂时不可用时，您的Workfront管理员可以登录Workfront。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">启用 </td> 
      <td> <p>在Workfront系统上激活SSO。 确保已向用户传达了登录说明。</p> <p>在Workfront中启用SSO配置后，必须为所有用户启用<strong>仅允许SAML 2.0身份验证</strong>设置，以便他们可以使用SSO。</p> <p>有关更新SSO用户的详细信息，请参阅<a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">更新单点登录的用户</a>。</p> <p>有关用户设置的详细信息，请参阅<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户的配置文件</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">确认配置 </td> 
      <td> 
      <p>单击<strong>测试连接</strong>以验证Workfront和SAML 2.0身份提供程序是否可以相互通信。 仅当您交换XML文件时，此连接才成功。
      </p> 
      <p>成功测试SAML 2.0身份提供程序与Workfront之间的链接后，您会看到一个与下图类似的屏幕。</p>
      <p><b>注意</b>：此屏幕显示在浏览器弹出窗口中，因此请确保禁用浏览器中的弹出窗口阻止程序。</p>
      <p>保存表中显示的信息以供以后使用。</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**&#x200B;以保存SAML 2.0配置。
