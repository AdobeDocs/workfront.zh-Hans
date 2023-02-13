---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: 更新用户以进行单点登录
description: 您可以更新用户，以便在Workfront中进行单点登录。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 1%

---

# 更新用户以进行单点登录

{{important-admin-console-onboard}}

在Adobe Workfront实例中启用单点登录(SSO)后，您可以使用SSO凭据登录Workfront。

如果您的现有系统中已填充与SSO凭据关联的用户，则可以通过将逗号分隔值(CSV)文件导入Workfront，将用户的ID导入Workfront。

有关将Workfront与单点登录系统集成的更多信息，请参阅 [Adobe Workfront中的单点登录概述](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


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

## SSO用户名

根据您使用的SSO解决方案，SSO环境中的用户名可以称为以下任意名称：

* SSO 用户名
* 联邦标识
* 联合用户名

在Workfront中，所有这些名称都存储在用户对象的SSO用户名字段中。

为了让您的用户能够使用其SSO凭据登录Workfront，您必须更新其配置文件以在其Workfront用户名之外还包含其SSO用户名。

作为Workfront管理员，您可以使用用户名列表在Workfront中导入，以批量更新Workfront用户的SSO用户名字段。 此列表必须包含Workfront用户ID(GUID)以及每个用户的相应SSO用户名，并且必须将其另存为CSV或TSV文件。 此过程会更新Workfront中的现有SSO用户名，或者添加新的SSO用户名（如果用户缺少用户名）。

## 准备导入文件 {#prepare-the-import-file}

您可以通过在Workfront中生成一份报告，报告所有用户必须更新其SSO用户名字段，以开始准备导入文件。

1. 在Workfront中构建用户报表。

   有关在Workfront中构建用户报表的说明，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 在报表中选择以下字段：

   | 名称 | Workfront用户的全名。 |
   |---|---|
   | ID | ID是Workfront字母数字GUID。 |
   | SSO 用户名 | 选择SSO用户名字段，以确保导入时不会覆盖任何用户名。 如果您的用户尚未针对SSO进行更新，则所有用户都应将此字段留空。 |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. 保存报表。
1. 单击 **导出** 并将报表导出到Excel。
1. 打开导出的Excel文件，然后开始在“SSO用户名”列的报表中为每个用户添加SSO用户名。

   >[!IMPORTANT]
   >
   >SSO用户名区分大小写。

1. 除 **ID** 和 **SSO用户名** 列。

1. 消除列标题，并确保报表顶部没有空行。

   您用于使用SSO用户名更新Workfront用户的文件必须只包含2列，顺序如下：

   * 第一列应显示Workfront用户ID(Workfront中的用户GUID)。
   * 第二列应包含SSO用户名，它显示在您的SSO系统中。
   * 列应该没有标题，并且名称列表顶部不应有任何空行。

      ![](assets/update-users-for-sso-csv-file-for-import.png)

1. 将报表另存为CSV或TSV文件。

## 更新用户的单点登录 {#update-your-users-for-sso}

更新SSO用户的过程可以将SSO用户名字段添加到您的Workfront用户（如果不存在），或者如果该字段中已有与用户关联的值，则更新该字段中的值。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统** then **更新用于单点登录的用户**.

1. 单击 **选择文件** 浏览您准备的文件。

   有关如何准备此文件的更多信息，请参阅 [准备导入文件](#prepare-the-import-file).

1. 选择保存在计算机上的文件，然后单击 **打开**.

   这允许所有用户使用其SSO凭据登录Workfront。

   的 **仅允许 `<SSO Configuration>` 身份验证** 为CSV中包含的所有用户启用了设置。

## 验证您用户的Workfront用户名的SSO

有关生成包含SSO用户名信息的用户报表的说明，请参阅 [准备导入文件](#prepare-the-import-file).

1. 运行包含SSO用户名信息的用户报表。

   请注意，已为每个用户填充SSO用户名列。

1. 确保“SSO用户名”列的值与您的SSO服务器上的SSO用户名匹配。
1. 如果“SSO用户名”列为空，请更新用户的SSO用户名。

   ![](assets/users-with-sso-field-updated.png)

   有关为SSO更新用户的说明，请参阅 [更新用户的单点登录](#update-your-users-for-sso).
