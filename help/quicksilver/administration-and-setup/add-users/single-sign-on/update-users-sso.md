---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: 更新单点登录用户
description: 您可以在Workfront中为单点登录更新用户。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 75fea812b4574191522af4721a013b57aa5d609f
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 2%

---

# 更新用户以进行单点登录

<!-- Audited: 1/2024 -->

{{important-admin-console-onboard}}

在您的Adobe Workfront实例中启用单点登录(SSO)后，您的用户可以使用其SSO凭据登录Workfront。

如果您现有的系统中已填充了与SSO凭据关联的用户，则可以通过将逗号分隔值(CSV)文件导入Workfront，将用户的ID导入Workfront。

有关将Workfront与SSO系统集成的更多信息，请参阅[Adobe Workfront中的单点登录概述](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)。


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

## SSO用户名

根据您使用的SSO解决方案，可以将SSO环境中的用户名称为以下任意名称：

* SSO 用户名
* 联邦标识
* 联合用户名

无论在SSO环境中调用了什么用户名，该字段的值都存储在User对象的SSO用户名字段中。

为了使用户能够使用其SSO凭据登录Workfront，除了其Workfront用户名之外，您必须更新其配置文件以包含其SSO用户名。

作为Workfront管理员，您可以通过将用户名列表导入Workfront，批量更新Workfront用户的SSO用户名字段。 此列表必须：

* 包含Workfront用户ID (GUID)以及每个用户的相应SSO用户名
* 另存为CSV或TSV文件。

此过程会更新Workfront中的现有SSO用户名，或者添加新的SSO用户名（如果用户缺少用户名）。

## 准备导入文件 {#prepare-the-import-file}

您可以通过在Workfront中构建所有用户的报告来开始准备导入文件，这些用户必须更新其SSO用户名字段。

1. 在Workfront中构建用户报表。

   有关在Workfront中构建用户报表的说明，请参阅[创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 在报表中选择以下字段：

   | 字段 | 解释 |
   |---|---|
   | 名称 | Workfront用户的全名。 |
   | ID | ID是Workfront的字母数字GUID。 |
   | SSO 用户名 | 添加SSO用户名字段以确保导入不会覆盖任何用户名。 如果您的用户尚未针对SSO进行更新，则此字段对于所有用户都应为空。 |

   ![具有SSO用户名但没有访问权限的用户](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. 保存报表。
1. 单击报告顶部的&#x200B;**导出**&#x200B;并将报告导出到Excel。
1. 打开导出的Excel文件，并在“SSO用户名”列中为报告中的每个用户添加SSO用户名。

   >[!IMPORTANT]
   >
   >SSO用户名区分大小写。

1. 删除Excel文件中的所有列（**ID**&#x200B;和&#x200B;**SSO用户名**&#x200B;列除外）。

1. 删除列标题并确保报表顶部没有空白行。

   用于更新SSO用户名为&#x200B;**的Workfront用户的文件必须**&#x200B;只包含2列，顺序如下：

   * 第一列必须显示Workfront用户ID(即在Workfront中找到的用户GUID)。
   * 第二列必须包含SSO用户名，它显示在您的SSO系统中。
   * 列不得有标题，名称列表顶部不得有任何空行。

     ![更新用户CSV](assets/update-users-for-sso-csv-file-for-import.png)

1. 将报表另存为CSV或TSV文件。

## 更新用户以使用SSO {#update-your-users-for-sso}

更新SSO用户的过程要么将SSO用户名字段添加到您的Workfront用户（如果该字段不存在），要么更新该字段中的值（如果已存在与该用户关联的值）。

{{step-1-to-setup}}

1. 单击&#x200B;**系统**，然后选择&#x200B;**更新SSO的用户**。

1. 单击&#x200B;**选择文件**&#x200B;浏览您准备的文件。

   有关如何准备此文件的详细信息，请参阅[准备导入文件](#prepare-the-import-file)。

1. 选择保存在计算机上的文件，然后单击&#x200B;**打开**。

   这会将SSO凭据插入Workfront，使所有用户都可以使用其SSO凭据登录到Workfront。

   已为CSV中包含的所有用户启用&#x200B;**仅允许`<SSO Configuration>`身份验证**&#x200B;设置。 这可确保用户必须通过SSO登录。

## 根据用户的Workfront用户名验证SSO

有关生成包含SSO用户名信息的用户报告的说明，请参阅[准备导入文件](#prepare-the-import-file)。

1. 运行包含SSO用户名信息的用户报告。

   请注意，系统会为每个用户填充SSO用户名列。

1. 确保“SSO用户名”列的值与SSO服务器上的SSO用户名匹配。
1. 如果SSO用户名列为空，请更新用户的SSO用户名。

   ![具有SSO字段的用户](assets/users-with-sso-field-updated.png)

   有关更新SSO用户的说明，请参阅[更新SSO用户](#update-your-users-for-sso)。
