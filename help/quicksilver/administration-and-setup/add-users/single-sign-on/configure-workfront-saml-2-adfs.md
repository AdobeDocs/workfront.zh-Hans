---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: 使用ADFS使用SAML 2.0配置Adobe Workfront
description: 您可以使用SAML 2.0启用对Workfront的身份验证。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# 使用ADFS使用SAML 2.0配置Adobe Workfront

{{important-admin-console-onboard}}

作为Adobe Workfront管理员，您可以将Workfront与安全断言标记语言(SAML) 2.0解决方案集成，以便在使用Active Directory联合身份验证服务(ADFS)的同时实现单点登录。

本指南重点介绍如何在不使用自动配置或属性映射的情况下设置ADFS。 我们建议您在设置任何自动配置之前完成设置并测试它。

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
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 启用使用SAML 2.0对Workfront的身份验证

要使用SAML 2.0启用对Workfront Web应用程序和Workfront移动应用程序的身份验证，请完成以下部分：

* [检索Workfront SSO元数据文件](#retrieve-the-workfront-sso-metadata-file)
* [配置信赖方信任](#configure-relying-party-trusts)
* [配置声明规则](#configure-claim-rules)
* [上载元数据文件并测试连接](#upload-the-metadata-file-and-test-the-connection)

### 检索Workfront SSO元数据文件 {#retrieve-the-workfront-sso-metadata-file}

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**系统** > **单点登录(SSO)**。
1. 在&#x200B;**类型**&#x200B;下拉菜单中，单击&#x200B;**SAML 2.0**&#x200B;以显示其他信息和选项。
1. 复制&#x200B;**元数据URL**&#x200B;之后显示的URL。
1. 继续下一节，[配置信赖方信任](#configure-relying-party-trusts)。

### 配置信赖方信任 {#configure-relying-party-trusts}

1. 使用Windows Server 2008 R2打开&#x200B;**ADFS管理器**（版本可能有所不同）。
1. 转到&#x200B;**开始。**
1. 单击&#x200B;**管理工具。**
1. 单击&#x200B;**ADFS 2.0管理。**
1. 选择&#x200B;**ADFS**&#x200B;并展开&#x200B;**信任关系**。
1. 右键单击&#x200B;**信赖方信任**，然后选择&#x200B;**添加信赖方信任**&#x200B;以启动添加信赖方信任向导。
1. 从&#x200B;**欢迎页面**，选择&#x200B;**开始**。
1. 在&#x200B;**选择日期Source**&#x200B;部分中，粘贴Workfront中的元数据URL。
1. 单击&#x200B;**下一步**。
1. 单击&#x200B;**确定**&#x200B;确认警告消息。
1. 在&#x200B;**指定显示名称**&#x200B;部分中，添加&#x200B;**显示名称**&#x200B;和&#x200B;**注释**&#x200B;以区分信任，然后单击&#x200B;**下一步**。
1. 选择&#x200B;**允许所有用户访问此信赖方**（或者，如果稍后要配置此内容，选择&#x200B;**无**）。
1. 单击&#x200B;**下一步**。

   这会将您转到&#x200B;**添加信任**&#x200B;准备就绪分区。

1. 继续下面的部分[配置声明规则](#configure-claim-rules)。

### 配置声明规则 {#configure-claim-rules}

1. 在&#x200B;**准备添加信任**&#x200B;部分中单击&#x200B;**下一步**，然后确保选中&#x200B;**打开“编辑声明规则”对话框**&#x200B;选项。

   这将允许您在以后的步骤中编辑报销申请规则。

1. 单击&#x200B;**关闭**。
1. 单击&#x200B;**添加规则。**
1. 选择&#x200B;**将LDAP属性作为声明发送**。
1. 单击&#x200B;**下一步**&#x200B;以显示&#x200B;**配置声明规则**&#x200B;步骤。
1. 指定配置声明规则的以下最低要求： （这将在用户设置中进入&#x200B;**Federation ID**，并用于区分登录者。）


   <table >                
      <tbody>
            <tr>
               <td>声明规则名称
               </td>
               <td>指定声明规则的名称。 例如，“Workfront”。</td>
            </tr>
            <tr>
               <td>属性存储</td>
               <td >从下拉菜单中选择<b>Active Directory</b>。</td>
            </tr>
            <tr>
               <td>LDAP属性</td>
               <td>这可以是任何类型的属性。 我们建议对此属性使用<b>SAM-Account-Name</b>。</td>
            </tr>
            <tr>
               <td>传出声明类型</td>
               <td>必须选择<b>名称ID</b>作为传出声明类型</td>
            </tr>
      </tbody>
   </table>

1. （可选）要建立自动预配，请在LDAP属性和传出声明类型中添加以下附加声明：

   * 名字
   * 姓氏
   * 电子邮件地址

1. 单击“完成”****，然后在下一个屏幕上单击“确定”****。
1. 右键单击新的&#x200B;**信赖方信任**，然后选择&#x200B;**属性**。
1. 选择&#x200B;**高级选项卡**。 在&#x200B;**安全哈希算法**&#x200B;下，选择SHA-1或SHA-256。

   >[!NOTE]
   >
   >您在安全哈希算法下选择的选项必须与Workfront中设置>系统>单点登录(SSO)下的安全哈希算法字段匹配。

1. 继续到以下部分[上载元数据文件并测试连接](#upload-the-metadata-file-and-test-the-connection)。

### 上载元数据文件并测试连接 {#upload-the-metadata-file-and-test-the-connection}

1. 打开浏览器并导航到`https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` 。

   这应该下载元数据文件FederationMetadata.xml文件。

1. 单击&#x200B;**填充身份提供程序元数据**&#x200B;中的字段&#x200B;**选择文件**，然后选择&#x200B;**FederationMetadata.xml**&#x200B;文件。

1. （可选）如果证书信息未使用元数据文件填充，您可以单独上传文件。 在&#x200B;**证书**&#x200B;部分中选择&#x200B;**选择文件**。

1. 单击&#x200B;**测试连接**。 如果设置正确，您应该会看到一个类似于以下所示的页面：

   ![SAML 2成功消息](assets/success-saml-2.png)

   >[!NOTE]
   >
   >如果要设置属性映射，请确保将属性从“测试连接”复制到“目录属性”。 有关详细信息，请参阅映射用户属性。

1. 选择&#x200B;**管理劐免**&#x200B;可允许Workfront管理员使用带有旁路URL的Workfront凭据登录。

   指向`<yourdomain>`.my.workfront.com/login的书签绕过重定向。

1. 选择&#x200B;**启用**&#x200B;框以启用配置。
1. 单击&#x200B;**保存**。

## 关于更新SSO的用户

按照本指南，**SSO用户名**&#x200B;将是他们的&#x200B;**Active Directory用户名**。

作为Workfront管理员，您可以批量更新SSO的用户。 有关更新SSO用户的详细信息，请参阅[更新单点登录的用户](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)。

作为Workfront管理员，您还可以手动分配一个Federation ID，以编辑用户的配置文件并填写Federation ID字段。 有关编辑用户的详细信息，请参阅[编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

>[!NOTE]
>
>编辑用户配置文件以包含联合ID时，选择&#x200B;**仅允许SAML 2.0身份验证**&#x200B;会删除使用旁路URL (`<yourdomain>`.my.workfront.com/login)登录Workfront的功能。
