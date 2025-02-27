---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: 在身份提供程序中更新SAML 2.0元数据
description: 您可以在身份提供程序中更新SAML 2.0元数据。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 0%

---

# 在身份提供程序中更新SAML 2.0元数据

{{important-admin-console-onboard}}

以下各节介绍在使用Active Directory联合身份验证服务(ADFS)作为身份提供程序时，如何更新安全声明标记语言(SAML) 2.0元数据。

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

## 使用ADFS作为您的身份提供程序

您可以在Adobe Workfront更新SAML 2.0证书之前或之后更新ADFS元数据。 如果选择在Workfront更新SAML 2.0证书之前更新ADFS元数据，则需要执行其他步骤。

* [更新您的ADFS元数据](#update-your-adfs-metadata)
* [强制更新ADFS元数据](#force-your-adfs-metadata-to-update)

### 更新ADFS元数据 {#update-your-adfs-metadata}

要将ADFS元数据设置为自动更新，请完成此部分中的步骤。

默认情况下，ADFS配置为自动检查其所有信赖方信任元数据的更新；但是，默认设置为仅每24小时轮询一次。 可以使用powershell命令更改此值。

1. 登录到ADFS服务器并打开ADFS管理控制台。
1. 在左侧面板中，展开&#x200B;**ADFS 2.0，**，然后展开&#x200B;**信任关系。**

1. 单击&#x200B;**信赖方信任**&#x200B;文件夹。
1. 选择您之前配置为与Workfront一起使用的信赖方信任，然后在右侧面板中，单击&#x200B;**从联合元数据更新**。
1. （视情况而定）如果此选项灰显（这意味着信赖方信任之前是使用元数据文件配置的），请完成以下操作。

   1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**设置**![齿轮设置图标](assets/gear-icon-settings.png)。

   1. 单击&#x200B;**系统** > **单点登录(SSO)**。

   1. 单击&#x200B;**编辑设置。**
   1. 单击&#x200B;**编辑配置**，然后在&#x200B;**类型**&#x200B;下拉列表中选择&#x200B;**SAML 2.0**。

   1. 复制&#x200B;**元数据URL**，它应该类似于以下内容：

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. 在ADFS服务器上，右键单击您之前配置的信赖方信任，然后单击&#x200B;**属性。**
   1. 单击&#x200B;**监视**&#x200B;选项卡，然后将从Workfront复制的URL粘贴到&#x200B;**信赖方的联合元数据URL**&#x200B;字段。

   1. 检查&#x200B;**监视信赖方**&#x200B;和&#x200B;**自动更新信赖方**&#x200B;的选项。

   1. 单击&#x200B;**确定。**
   1. 选择您之前配置为与Workfront一起使用的信赖方信任；然后在右侧面板中，单击&#x200B;**从联合元数据更新。**

1. 单击&#x200B;**确定**&#x200B;忽略有关ADFS 2.0不支持的联合元数据中某些内容的消息。
1. 打开&#x200B;**Windows Powershell模块。**
1. 加载所有模块后，在powershell中运行以下命令：

   `Get-ADFSProperties`

1. 查找&#x200B;**监视间隔**&#x200B;旁边的值。

   它将是一个数字，表示两次投票之间的分钟数。 默认值应为1440（1440分钟= 24小时）。

1. 通过在powershell中运行以下命令来设置新值：

   `Set-ADFSProperties -MonitoringInterval 1`

   这会将监控间隔从每24小时更改为每分钟。 如果希望较少轮询，可以将1更改为另一个较大的值。

1. 要验证此功能是否正常工作，请使用&#x200B;**事件查看器**&#x200B;在ADFS2.0日志中查找以下信息：

   **事件ID 156和157**

### 强制更新ADFS元数据 {#force-your-adfs-metadata-to-update}

要更新ADFS元数据，请完成以下部分中的步骤。

要在使用Active Directory联合身份验证服务(ADFS)时强制在Workfront和SAML 2.0提供程序之间交换元数据，请执行以下操作：

>[!NOTE]
>
>其中一些更改可能需要由您的IT部门来完成。

1. 登录到ADFS服务器并打开&#x200B;**ADFS管理控制台**。
1. 在左侧面板中，展开&#x200B;**ADFS 2.0**，然后展开&#x200B;**信任关系**。

1. 单击&#x200B;**信赖方信任**&#x200B;文件夹。
1. 选择您之前配置为与Workfront一起使用的信赖方信任，然后在右侧面板中，单击&#x200B;**从联合元数据更新**。

   如果此选项灰显且无法选择，请完成以下操作：

   （仅当之前使用元数据文件配置了信赖方信任时，选项才会灰显。）

   1. 在Workfront的“设置”区域中，从Workfront单点登录设置屏幕复制&#x200B;**元数据URL**。

      要访问&#x200B;**元数据URL**&#x200B;的信息，请执行以下操作：

      1. 单击全局导航栏上Adobe Workfront右上角附近的&#x200B;**设置**。
      1. 单击> **系统** > **单点登录(SSO)**。
      1. 单击&#x200B;**编辑设置。**
      1. 单击&#x200B;**编辑配置**，然后在&#x200B;**类型**&#x200B;下拉列表中选择&#x200B;**SAML 2.0**。
      1. 复制&#x200B;**元数据URL**，它应该类似于以下内容：

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. 在ADFS服务器上，右键单击您之前配置的信赖方信任，然后单击&#x200B;**属性。**
   1. 单击&#x200B;**监视**&#x200B;选项卡，然后将从Workfront复制的URL粘贴到&#x200B;**信赖方的联合元数据URL**&#x200B;字段。
   1. 检查&#x200B;**监视信赖方**&#x200B;和&#x200B;**自动更新信赖方**&#x200B;的选项。
   1. 单击&#x200B;**确定**。
   1. 选择您之前配置为与Workfront一起使用的信赖方信任，然后在右侧面板中，单击&#x200B;**从联合元数据更新。**

1. 单击&#x200B;**确定**&#x200B;忽略有关ADFS 2.0不支持的联合元数据中某些内容的消息。
1. 单击&#x200B;**更新**&#x200B;以完成更新联合元数据。

允许使用Workfront登录凭据（可在&#x200B;**访问**&#x200B;部分中的每个用户的配置文件页面中进行配置）通过本机登录屏幕访问Workfront的用户，可通过导航到以下URL使用其Workfront用户名和密码登录： `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`。

## 使用其他身份提供程序

使用ADFS以外的身份提供程序（例如Ping、Okta或Centrify）时，必须将Workfront元数据重新上传到身份提供程序。

有关如何获取新的Workfront元数据URL的详细信息，请参阅[更新您的ADFS元数据](#update-your-adfs-metadata)。

有关在Workfront中将Active Directory联合身份验证服务(ADFS)与SAML 2.0结合使用的其他信息，请参阅[使用ADFS在Adobe Workfront中配置SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)。
