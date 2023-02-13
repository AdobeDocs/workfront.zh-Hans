---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: 在您的身份提供程序中更新SAML 2.0元数据
description: 您可以在身份提供程序中更新SAML 2.0元数据。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 96f1d50024605328713ca2019f3b726e27dc569c
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---

# 在您的身份提供程序中更新SAML 2.0元数据

{{important-admin-console-onboard}}

以下各节介绍了在使用Active Directory联合身份验证服务(ADFS)作为身份提供程序时如何更新您的安全断言标记语言(SAML)2.0元数据。

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

## 使用ADFS作为身份提供者

您可以在Adobe Workfront更新SAML 2.0证书之前或之后更新ADFS元数据。 如果在Workfront更新SAML 2.0证书之前选择更新ADFS元数据，则需要执行其他步骤。

* [更新ADFS元数据](#update-your-adfs-metadata)
* [强制更新ADFS元数据](#force-your-adfs-metadata-to-update)

### 更新ADFS元数据 {#update-your-adfs-metadata}

要将ADFS元数据设置为自动更新，请完成此部分中的步骤。

默认情况下，ADFS配置为自动检查其所有信赖方信任元数据的更新；但是，默认设置为仅每24小时进行一次轮询。 您可以使用powershell命令更改此值。

1. 登录到ADFS服务器并打开ADFS管理控制台。
1. 在左侧面板中，展开 **ADFS 2.0、** 然后展开 **信任关系。**

1. 单击 **信赖方信托** 文件夹。
1. 选择您之前配置为与Workfront一起使用的信赖方信任，然后在右侧面板中，单击&#x200B;**从联合元数据更新**.
1. （视情况而定）如果此选项灰显（这表示信赖方信任以前是使用元数据文件配置的），请完成以下操作。

   1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

   1. 单击 **系统** > **单点登录(SSO)**.

   1. 单击 **编辑设置。**
   1. 单击 **编辑配置**，然后选择 **SAML 2.0** 在 **类型** 下拉列表。

   1. 复制 **元数据URL**，它应类似于以下内容：

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. 在ADFS服务器上，右键单击您之前配置的信赖方信任，然后单击 **属性。**
   1. 单击 **监控** ，然后将您从Workfront复制的URL粘贴到 **依赖方的联合元数据URL** 字段。

   1. 选中选项以 **监视依赖方** 和 **自动更新信赖方**.

   1. 单击 **好。**
   1. 选择您之前配置为与Workfront一起使用的信赖方信任；然后，在右侧面板中，单击 **从联合元数据更新。**

1. 单击 **确定** 忽略ADFS 2.0不支持的联合元数据中某些内容的消息。
1. 打开 **Windows Powershell模块。**
1. 在加载所有模块后，在powershell中运行以下命令：

   `Get-ADFSProperties`

1. 在 **监控间隔。**

   它将是一个数字，表示两次投票之间的分钟数。 默认时间应为1440（1440分钟= 24小时）。

1. 通过在powershell中运行以下命令来设置新值：

   `Set-ADFSProperties -MonitoringInterval 1`

   这会将监控间隔从每24小时更改为每分钟一次。 如果希望轮询频率较低，可以将1更改为另一个较大的值。

1. 要验证其是否正常工作，请使用 **事件查看器** 要在ADFS2.0日志中查找以下信息，请执行以下操作：

   **事件ID 156和157**

### 强制更新ADFS元数据 {#force-your-adfs-metadata-to-update}

要更新ADFS元数据，请完成以下部分中的步骤。

在使用Active Directory联合身份验证服务(ADFS)时，要强制在Workfront与SAML 2.0提供程序之间交换元数据，请执行以下操作：

>[!NOTE]
>
>其中一些更改可能需要由您的IT部门完成。

1. 登录到ADFS服务器并打开 **ADFS管理控制台**.
1. 在左侧面板中，展开 **ADFS 2.0**，然后展开 **信任关系**.

1. 单击 **信赖方信托** 文件夹。
1. 选择您之前配置为与Workfront一起使用的信赖方信任，然后在右侧面板中，单击 **从联合元数据更新**.

   如果此选项灰显且无法选择，请完成以下操作：

   （仅当先前使用元数据文件配置了信赖方信任时，此选项才会灰显。）

   1. 在Workfront的“设置”区域中，复制 **元数据URL** 从Workfront单点登录设置屏幕。

      访问 **元数据URL**:

      1. 单击 **设置** 在Adobe Workfront的右上角附近。
      1. 单击> **系统** > **单点登录(SSO)**.
      1. 单击 **编辑设置。**
      1. 单击 **编辑配置**，然后选择 **SAML 2.0** 在 **类型** 下拉列表。
      1. 复制 **元数据URL**，它应类似于以下内容：

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`
   1. 在ADFS服务器上，右键单击您之前配置的信赖方信任，然后单击 **属性。**
   1. 单击 **监控** ，然后将您从Workfront复制的URL粘贴到 **依赖方的联合元数据URL** 字段。
   1. 选中选项以 **监视依赖方** 和 **自动更新信赖方**.
   1. 单击 **确定**.
   1. 选择您之前配置为与Workfront一起使用的信赖方信任，然后在右侧面板中，单击 **从联合元数据更新。**


1. 单击 **确定** 忽略ADFS 2.0不支持的联合元数据中某些内容的消息。
1. 单击 **更新** 以完成联合元数据的更新。

允许使用Workfront登录凭据通过本机登录屏幕访问Workfront的用户(可在 **访问** 部分)可以通过导航到以下URL，使用其Workfront用户名和密码登录： `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## 使用其他身份提供程序

使用ADFS以外的身份提供程序（例如Ping、Okta或Centrify）时，必须将Workfront元数据重新上传到您的身份提供程序。

有关如何获取新的Workfront元数据URL的更多信息，请参阅 [更新ADFS元数据](#update-your-adfs-metadata).

有关在Workfront中将Active Directory联合身份验证服务(ADFS)与SAML 2.0结合使用的其他信息，请参阅 [使用ADFS使用SAML 2.0配置Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
