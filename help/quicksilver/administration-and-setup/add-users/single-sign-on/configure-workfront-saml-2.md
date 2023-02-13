---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: 使用SAML 2.0配置Adobe Workfront
description: 作为Adobe Workfront管理员，您可以配置Workfront Web和移动应用程序，以与用于单点登录(SSO)的安全断言标记语言(SAML)2.0解决方案相集成。
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 7%

---

# 使用SAML 2.0配置Adobe Workfront

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

{{important-admin-console-onboard}}

作为Adobe Workfront管理员，您可以配置Workfront Web和移动应用程序，以与用于单点登录(SSO)的安全断言标记语言(SAML)2.0解决方案相集成。

在Workfront中配置SAML 2.0（如以下各节所述）后，您可以维护配置，如 [在您的身份提供程序中更新SAML 2.0元数据](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

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

## 使用SAML 2.0启用对Workfront的身份验证

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统** > **单点登录(SSO)。**

1. 在 **类型** 下拉列表中，单击 **SAML 2.0。**

1. 在显示的选项顶部附近，单击 **下载SAML 2.0元数据** 下载您计算机上的文件。

   您的SAML 2.0身份提供程序需要一个XML文件，其中包含在您的Workfront实例中生成的信息。 下载文件后，您需要转到SAML 2.0身份提供程序服务器，并将Workfront SAML 2.0元数据XML文件上载到该服务器。

1. 指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">服务提供者标识 </td> 
      <td> 此URL已为您填充，用于向您的标识提供者标识Workfront。 例如： <code>&lt;yourcompany&gt;.com/SAML2</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">绑定类型</span> </td> 
      <td> <p>选择IDP服务器支持的用于发送身份验证信息的方法：</p> 
       <ul> 
        <li>POST</li> 
        <li>重定向</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">填充身份提供程序元数据中的字段 </td> 
      <td>在SAML 2.0身份提供程序解决方案中，导出服务提供程序元数据XML文件，并将其保存到计算机上的临时位置。 选择 <strong>选择文件</strong>，然后查找并选择您保存的文件以将其添加到Workfront配置。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">登录入口 URL</span> </td> 
      <td>指定贵组织的常用登录门户。 这是用户登录以访问Workfront以及与SAML 2.0集成的所有其他应用程序的URL。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">登出 URL</span> </td> 
      <td> <p>指定IDP服务器的注销URL。 Workfront在注销Workfront之前会向此URL发送HTTP请求。 当Workfront会话关闭时，这将关闭远程服务器上用户的会话。</p> <p><b>注意</b>:仅当您在用户配置文件中启用了“仅允许SAML 2.0身份验证”选项时，您才会被重定向到注销URL。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">更改密码 URL </td> 
      <td> <p> 指定用户将被重定向以更改其密码的URL。 </p> <p>由于SAML 2.0凭据用于访问Workfront，因此用户需要重定向到一个页面，以便在该页面中更改其SAML 2.0密码，而不是通过Workfront完成此活动。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">安全哈希算法 </td> 
      <td> <p>选择IDP支持的安全哈希算法(SHA):</p> 
       <ul> 
        <li>SHA-1</li> 
        <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自动预配置用户</span> </td> 
      <td> <p>当具有目录用户名和密码的新用户首次尝试登录Workfront时，会自动在系统中创建用户。</p> <p>要在Workfront中创建用户，您需要将Workfront数据属性与目录提供程序中的以下用户数据属性映射：</p> 
       <ul> 
        <li>姓</li> 
        <li>名</li> 
        <li>电子邮件地址</li> 
       </ul> 
       <p>将显示以下选项以允许您执行此操作：</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>从下拉列表中选择要映射的Workfront用户属性，然后在用户目录中指定相应的目录属性。</p> 
       <p>的 <strong>目录属性</strong> 字段应包含在成功测试SAML 2.0配置时保存的“用户属性”表中的“目录属性名称”。</p> 
       <p>您可以在 <strong>默认值</strong> 字段。 您还可以根据SAML 2.0身份提供程序中的值设置规则。</p> 
       <p><b>警告</b>:Workfront会在用户每次登录系统时尝试映射下面列出的属性。 因此，我们不建议映射访问级别。 如果属性映射不正确，您可以轻松删除管理访问权限。 单击添加映射以添加其他规则。
       </p> 
       <p>您可以映射以下Workfront属性：</p> 
      <ul> 
      <li> <p>访问级别</p> </li> 
      <li> <p>地址</p> </li> 
      <li> <p>地址 2</p> </li> 
      <li> <p>记帐/小时</p> </li> 
      <li> <p>城市</p> </li> 
      <li> <p>公司</p> </li> 
      <li> <p>成本/小时</p> </li> 
      <li> <p>电子邮件地址</p> </li> 
      <li> <p>分机</p> </li> 
      <li> <p>姓</p> </li> 
      <li> <p>主组</p> </li> 
      <li> <p>主团队</p> </li> 
      <li> <p>工作角色</p> </li> 
      <li> <p>名</p> </li> 
      <li> <p>布局模板</p> </li> 
      <li> <p>经理</p> </li> 
      <li> <p>手机</p> </li> 
      <li> <p>电话号码</p> </li> 
      <li> <p>邮政编码</p> </li> 
      <li> <p>计划</p> </li> 
      <li> <p>州/省</p> </li> 
      <li> <p>时间表配置文件</p> </li> 
      <li> <p>标题</p> </li> 
      </ul> </td> 
          <td> </td> 
         </tr> 
        </tbody> 
        <p>单击 <strong>保存</strong> 完成映射用户属性时。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">证书 </td> 
      <td> <p>上载有效的SSL证书，以确保身份验证服务与Workfront之间的安全连接。 对于OnDemand帐户，始终需要证书。 您可以从SAML 2.0系统管理员处获取此证书。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理豁免 </td> 
      <td> <p>允许Workfront管理员使用其Workfront登录名访问Workfront。 如果未选择此选项，Workfront管理员必须使用其SAML 2.0用户名和密码。</p> 
      <p>Workfront首先尝试通过SAML 2.0为具有Workfront系统管理员访问级别的用户登录Workfront。 如果SAML 2.0身份验证失败，Workfront将对Workfront管理员使用本地身份验证。</p> 
      <p>我们建议您始终选择此选项，以便当SAML 2.0提供程序暂时不可用时，Workfront管理员可以登录Workfront。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">启用 </td> 
      <td> <p>在Workfront系统上激活单点登录。 确保您已向用户传达了登录说明。</p> <p>在Workfront中启用SSO配置后，必须启用 <strong>仅允许SAML 2.0身份验证</strong> 为所有用户设置，以便他们可以使用单点登录。</p> <p>有关更新用于SSO的用户的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">更新用户以进行单点登录</a>.</p> <p>有关用户设置的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户的配置文件</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">确认配置 </td> 
      <td> 
      <p>单击 <strong>测试连接</strong> 以验证Workfront和SAML 2.0身份提供程序是否可以相互通信。 仅当您交换XML文件时，此连接才成功。
      </p> 
      <p>成功测试SAML 2.0身份提供程序与Workfront之间的链接后，您会看到与下面类似的屏幕。</p>
      <p><b>注意</b>:此屏幕显示在浏览器弹出窗口中，因此请确保您在浏览器中禁用弹出窗口阻止程序。</p>
      <p>保存表中显示的信息，供以后使用。</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **保存** 保存SAML 2.0配置。
