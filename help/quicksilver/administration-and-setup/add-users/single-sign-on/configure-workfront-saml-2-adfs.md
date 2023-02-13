---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: 使用ADFS使用SAML 2.0配置Adobe Workfront
description: 您可以使用SAML 2.0启用对Workfront的身份验证。
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# 使用ADFS使用SAML 2.0配置Adobe Workfront

{{important-admin-console-onboard}}

作为Adobe Workfront管理员，您可以在使用Active Directory联合身份验证服务(ADFS)时，将Workfront与安全断言标记语言(SAML)2.0解决方案集成，以实现单点登录。

本指南重点介绍如何在不自动配置或属性映射的情况下设置ADFS。 我们建议您在设置任何自动配置之前完成设置并测试它。

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

要使用SAML 2.0对Workfront Web应用程序和Workfront移动应用程序启用身份验证，请完成以下部分：

* [检索Workfront SSO元数据文件](#retrieve-the-workfront-sso-metadata-file)
* [配置信赖方信托](#configure-relying-party-trusts)
* [配置声明规则](#configure-claim-rules)
* [上传元数据文件并测试连接](#upload-the-metadata-file-and-test-the-connection)

### 检索Workfront SSO元数据文件 {#retrieve-the-workfront-sso-metadata-file}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).
1. 在左侧面板中，单击 **系统** > **单点登录(SSO)**.
1. 在 **类型** 下拉菜单中，单击 **SAML 2.0** 以显示其他信息和选项。
1. 复制在 **元数据URL**.
1. 继续执行以下部分： [配置信赖方信托](#configure-relying-party-trusts).

### 配置信赖方信托 {#configure-relying-party-trusts}

1. 打开 **ADFS管理器** 使用Windows server 2008 R2（版本可能有所不同）。
1. 转到 **开始。**
1. 单击 **管理工具。**
1. 单击 **ADFS 2.0管理。**
1. 选择 **ADFS** 展开 **信任关系**.
1. 右键单击 **信赖方信托**，然后选择 **添加信赖方信任** 启动“添加信赖方信任向导”。
1. 从 **欢迎页面**，选择 **开始**.
1. 在 **选择日期来源** 部分，粘贴Workfront中的元数据URL。
1. 单击 **下一个**.
1. 单击 **确定** 以确认警告消息。
1. 在 **指定显示名称** 部分，添加 **显示名称** 和 **注释** 要区分信任，请单击 **下一个**.
1. 选择 **允许所有用户访问此信赖方** (或 **无** （如果以后要配置）。
1. 单击 **下一个**.

   这会将您转到 **准备添加信任** 中。

1. 继续执行以下部分 [配置声明规则](#configure-claim-rules).

### 配置声明规则 {#configure-claim-rules}

1. 单击 **下一个** 在 **准备添加信任** 部分，然后确保 **打开“编辑声明规则”对话框** 选项。

   这样，您就可以在以后的步骤中编辑声明规则。

1. 单击&#x200B;**关闭**。
1. 单击 **添加规则。**
1. 选择 **将LDAP属性作为声明发送**.
1. 单击 **下一个** 以显示 **配置声明规则** 中。
1. 指定以下最低要求以配置声明规则：(这将在 **联合ID** ，用于区分登录者。)


   <table >                
      <tbody>
            <tr>
               <td>声明规则名称
               </td>
               <td>指定声明规则的名称。 例如，“Workfront”。</td>
            </tr>
            <tr>
               <td>属性存储</td>
               <td >选择 <b>Active Directory</b> 下拉菜单中。</td>
            </tr>
            <tr>
               <td>LDAP属性</td>
               <td>这可以是任何类型的属性。 我们建议使用 <b>SAM-Account-Name</b> 属性。</td>
            </tr>
            <tr>
               <td>传出声明类型</td>
               <td>您必须选择 <b>名称ID</b> 作为传出索赔类型</td>
            </tr>
      </tbody>
   </table>

1. （可选）要建立自动设置，请在LDAP属性和传出声明类型中添加以下附加声明：

   * 给定名称
   * 姓氏
   * 电子邮件地址

1. 单击 **完成**，然后单击 **确定** 在下一个屏幕上。
1. 右键单击新 **信赖方信任**，然后选择 **属性**.
1. 选择&#x200B;**“高级”选项卡**. 和下 **安全哈希算法** 选择SHA-1或SHA-256。

   >[!NOTE]
   >
   >您在安全哈希算法下选择的选项必须与Workfront中设置>系统>单点登录(SSO)下的安全哈希算法字段匹配。

1. 继续执行以下部分 [上传元数据文件并测试连接](#upload-the-metadata-file-and-test-the-connection).

### 上传元数据文件并测试连接 {#upload-the-metadata-file-and-test-the-connection}

1. 打开浏览器并导航到 `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` .

   这应该下载元数据文件FederationMetadata.xml文件。

1. 单击 **选择文件** 在 **从身份提供程序元数据填充字段**，然后选择 **FederationMetadata.xml** 文件。

1. （可选）如果证书信息没有使用元数据文件进行填充，则可以单独上传文件。 选择 **选择文件** 在 **证书** 中。

1. 单击 **测试连接**. 如果设置正确，您应会看到与下面所示类似的页面：

   ![](assets/success-saml-2.png)

   >[!NOTE]
   >
   >如果要设置属性映射，请确保将Test Connection中的属性复制到目录属性中。 有关更多信息，请参阅映射用户属性。

1. 选择 **管理员免除** 以允许Workfront管理员通过绕过url使用Workfront凭据登录。

   指向的书签 `<yourdomain>`.my.workfront.com/login绕过重定向。

1. 选择 **启用** 框中，选择要启用配置的复选框。
1. 单击&#x200B;**保存**。

## 关于更新SSO用户

根据本指南， **SSO用户名** 将是他们的 **Active Directory用户名**.

作为Workfront管理员，您可以批量更新SSO用户。 有关更新用于SSO的用户的更多信息，请参阅 [更新用户以进行单点登录](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

作为Workfront管理员，您还可以手动分配联合ID，以编辑用户的配置文件并填写联合ID字段。 有关编辑用户的更多信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>在编辑用户的配置文件以包含联合ID时，选择 **仅允许SAML 2.0身份验证** 删除了使用绕过url(`<yourdomain>`.my.workfront.com/login)。
