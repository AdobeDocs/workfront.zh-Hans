---
title: 增强型身份验证概述
description: 在搜索和左侧导航中隐藏
hidefromtoc: true
hide: true
feature: System Setup and Administration
role: Admin
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 4%

---

# 增强型身份验证概述

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront正在更改用户和密码的系统管理。 这些更改将在名为&#x200B;**增强型身份验证**&#x200B;体验的分阶段版本中推出。 增强的身份验证功能可在所有Workfront产品和服务中为用户提供更一致和更安全的登录体验。

下表提供了有关当前和未来功能的详细信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>功能</strong> </p> </th> 
   <th><strong>旧身份验证</strong> </th> 
   <th><strong>增强型身份验证1.0</strong> </th> 
   <th> <p>增强型身份验证2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>登录选项</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>启用一个用户名用于所有Workfront产品和服务，包括培训、支持及其他</p> </td> 
   <td>不可用</td> 
   <td> <p>不可用</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>允许在Workfront实例中使用相同的电子邮件地址</p> </td> 
   <td> <p>✓</p> <p>自2019.3版本起可用</p> </td> 
   <td> <p>✓</p> <p>自2019.3版本起可用</p> </td> 
   <td> <p>✓</p> <p>自2019.3版本起可用</p> </td> 
  </tr> 
  <tr> 
   <td> <p>电子邮件地址区分大小写</p> </td> 
   <td> <p>✓</p> <p>自2019.3版本起可用</p> </td> 
   <td> <p>✓</p> <p>如果地址仅按大小写不同，则多个用户不能具有相同的电子邮件地址。 </p> </td> 
   <td> <p>✓</p> <p>如果地址仅按大小写不同，则多个用户不能具有相同的电子邮件地址。 </p> <p>我们将在2019年底通知Workfront管理员开始修复重复的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>密码管理选项</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>为作为Workfront管理员的用户启动密码重置电子邮件</p> </td> 
   <td> <p>不可用 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>为用户设置Workfront管理员临时密码</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>未计划</p> <p>此功能不是最佳安全实践</p> </td> 
   <td> <p>未计划</p> <p>此功能不是最佳安全实践</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>密码策略要求</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>要求用户在特定时间范围后重置密码</p> </td> 
   <td>✓</td> 
   <td> <p>未计划</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>限制用户使用以前的密码 </p> </td> 
   <td>✓</td> 
   <td>未计划 </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>防止错误密码输入尝试 </p> </td> 
   <td> <p>✓ </p> <p>在5次密码输入尝试不正确后锁定帐户。 Workfront管理员配置锁定后所需的等待时间</p> </td> 
   <td> <p>✓</p> <p>根据行业最佳实践，在每次连续输入错误密码后，等待时间会以指数形式增加；Workfront管理员无法配置所需的时间</p> </td> 
   <td> <p>✓</p> <p>使用锁定算法，主动阻止各种可疑行为。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>需要混合使用小写、大写、数字和特殊字符</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>提高了选择特定需求的灵活性</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>设置最小密码长度 </p> </td> 
   <td> 不可用 </td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Restrict users from using more than 2 identical characters in a row</td> 
    <td>Not available</td> 
    <td>Not available</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
  <tr> 
   <td colspan="3"> <p><strong>单点登录协议支持</strong></p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>支持与Active Directory和LDAP协议兼容的SSO集成</p> </td> 
   <td> ✓ </td> 
   <td> <p> 已弃用</p> <p>Active Directory、Azure和LDAP系统应使用SAML 2.0</p> </td> 
   <td> <p>已弃用</p> <p>Active Directory、Azure和LDAP系统可以使用加密的SAML 2.0或OpenID Connect进行配置。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>支持与SAML 2.0兼容的SSO协议 </p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>支持开放ID连接协议</p> </td> 
   <td> <p>不可用</p> </td> 
   <td> <p>不可用</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> 将Workfront登录页面配置为始终重定向到身份提供程序登录页面 </p> </td> 
   <td> 默认启用，无法禁用</td> 
   <td> <p>✓</p> <p>Workfront管理员可以将“登录”页配置为重定向到“身份提供程序”登录页，也可以配置登录按钮。</p> </td> 
   <td> <p>✓</p> <p> Workfront管理员可以配置登录页面以重定向到身份提供程序的登录页面，也可以配置登录按钮。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>允许每个实例启用多个SSO提供程序</p> </td> 
   <td> <p>不适用</p> </td> 
   <td> <p>未计划</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>环境支持</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>预览环境的单个用户名和密码</p> </td> 
   <td> <p>不可用</p> </td> 
   <td> <p>不可用</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>沙盒环境的单个用户名和密码</p> </td> 
   <td> <p>不可用</p> </td> 
   <td> <p>不可用</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr> 
    <td> <p>Available for Production environments</p> </td> 
    <td>✓</td> 
    <td> ✓&nbsp;</td> 
    <td> <p>✓</p> </td> 
   </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> Available for Preview and Sandbox environments&nbsp;</td> 
    <td> ✓&nbsp;</td> 
    <td> ✓</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>
