---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: 在身份提供程序中更新SAML 2.0元数据
description: 您可以在身份提供程序中更新SAML 2.0元数据。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '994'
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
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 使用ADFS作为您的身份提供程序

您可以在Adobe Workfront更新SAML 2.0证书之前或之后更新ADFS元数据。 如果选择在Workfront更新SAML 2.0证书之前更新ADFS元数据，则需要执行其他步骤。

* [更新ADFS元数据](#update-your-adfs-metadata)
* [强制更新ADFS元数据](#force-your-adfs-metadata-to-update)

### 更新ADFS元数据 {#update-your-adfs-metadata}

要将ADFS元数据设置为自动更新，请完成此部分中的步骤。

默认情况下，ADFS配置为自动检查其所有信赖方信任元数据的更新；但是，默认设置为仅每24小时轮询一次。 可以使用powershell命令更改此值。

1. 登录到ADFS服务器并打开ADFS管理控制台。
1. 在左侧面板中，展开 **ADFS 2.0、** 然后展开 **信任关系。**

1. 单击 **信赖方信任** 文件夹。
1. 选择您之前配置为与Workfront一起使用的信赖方信任，然后在右侧面板中，单击&#x200B;**从联合元数据更新**.
1. （视情况而定）如果此选项灰显（这意味着信赖方信任之前是使用元数据文件配置的），请完成以下操作。

   1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

   1. 单击 **系统** > **单点登录(SSO)**.

   1. 单击 **编辑设置。**
   1. 单击 **编辑配置**，然后选择 **SAML 2.0** 在 **类型** 下拉列表。

   1. 复制 **元数据URL**，它应类似于以下内容：

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. 在ADFS服务器上，右键单击您之前配置的信赖方信任，然后单击 **属性。**
   1. 单击 **监控** 选项卡，然后将您从Workfront复制的URL粘贴到 **信赖方的联合元数据URL** 字段。

   1. 选中选项以 **监视信赖方** 和 **自动更新信赖方**.

   1. 单击 **好的。**
   1. 选择您之前配置为与Workfront一起使用的信赖方信任；然后在右侧面板中，单击 **从联合元数据更新。**

1. 单击 **确定** 忽略有关ADFS 2.0不支持的联合元数据中某些内容的消息。
1. 打开 **Windows Powershell模块。**
1. 加载所有模块后，在powershell中运行以下命令：

   `Get-ADFSProperties`

1. 查找旁边的值 **监视间隔。**

   它将是一个数字，表示两次投票之间的分钟数。 默认值应为1440（1440分钟= 24小时）。

1. 通过在powershell中运行以下命令来设置新值：

   `Set-ADFSProperties -MonitoringInterval 1`

   这会将监控间隔从每24小时更改为每分钟。 如果希望较少轮询，可以将1更改为另一个较大的值。

1. 要验证此功能是否正常工作，请使用 **事件查看器** 在ADFS2.0日志中查找以下信息：

   **事件ID 156和157**

### 强制更新ADFS元数据 {#force-your-adfs-metadata-to-update}

要更新ADFS元数据，请完成以下部分中的步骤。

要在使用Active Directory联合身份验证服务(ADFS)时强制在Workfront和SAML 2.0提供程序之间交换元数据，请执行以下操作：

>[!NOTE]
>
>其中一些更改可能需要由您的IT部门来完成。

1. 登录到ADFS服务器并打开 **ADFS管理控制台**.
1. 在左侧面板中，展开 **ADFS 2.0**，然后展开 **信任关系**.

1. 单击 **信赖方信任** 文件夹。
1. 选择您之前配置为与Workfront一起使用的信赖方信任，然后在右侧面板中，单击 **从联合元数据更新**.

   如果此选项灰显且无法选择，请完成以下操作：

   （仅当之前使用元数据文件配置了信赖方信任时，选项才会灰显。）

   1. 在Workfront的“设置”区域中，复制 **元数据URL** 从您的Workfront单点登录设置屏幕中。

      要访问 **元数据URL**：

      1. 单击 **设置** 位于全局导航栏上Adobe Workfront的右上角附近。
      1. 单击> **系统** > **单点登录(SSO)**.
      1. 单击 **编辑设置。**
      1. 单击 **编辑配置**，然后选择 **SAML 2.0** 在 **类型** 下拉列表。
      1. 复制 **元数据URL**，它应类似于以下内容：

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. 在ADFS服务器上，右键单击您之前配置的信赖方信任，然后单击 **属性。**
   1. 单击 **监控** 选项卡，然后将您从Workfront复制的URL粘贴到 **信赖方的联合元数据URL** 字段。
   1. 选中选项以 **监视信赖方** 和 **自动更新信赖方**.
   1. 单击 **确定**.
   1. 选择您之前配置为与Workfront一起使用的信赖方信任，然后在右侧面板中，单击 **从联合元数据更新。**

1. 单击 **确定** 忽略有关ADFS 2.0不支持的联合元数据中某些内容的消息。
1. 单击 **更新** 完成更新联合元数据。

允许使用Workfront登录凭据通过本机登录屏幕访问Workfront的用户(这可以从以下位置中每个用户的配置文件页面进行配置 **访问** 部分)可以通过导航到以下URL，使用其Workfront用户名和密码登录： `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## 使用其他身份提供程序

使用ADFS以外的身份提供程序（例如Ping、Okta或Centrify）时，必须将Workfront元数据重新上传到身份提供程序。

有关如何获取新的Workfront元数据URL的更多信息，请参阅 [更新ADFS元数据](#update-your-adfs-metadata).

有关在Workfront中将Active Directory联合身份验证服务(ADFS)与SAML 2.0结合使用的其他信息，请参阅 [使用ADFS使用SAML 2.0配置Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
