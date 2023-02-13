---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart，kickstart，kickstarts，kickstarts
navigation-topic: use-kick-starts
title: ‘启动方案：公司、组、角色和用户启动准备’
description: 在开始实施Adobe Workfront时，您可以导入客户列表、内部部门、职务角色和用户信息，而不是手动输入数据。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 10%

---

# 启动方案：公司、组、角色和用户启动准备

在开始实施Adobe Workfront时，您可以导入客户列表、内部部门、职务角色和用户信息，而不是手动输入数据。

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

## 可导入的内容

下表显示了要导入的公司、组和角色：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>公司</strong> </th> 
   <th><strong>组</strong> </th> 
   <th><strong>角色</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td valign="top"> <p>Acme， Co</p> <p>Workfront公司</p> <p><em>您的公司</em> </p> <p>XYZ， Inc.</p> </td> 
   <td valign="top"> <p valign="top" rowspan="7">财务</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">营销 </p> <p valign="top" rowspan="7">销售</p> </td> 
   <td valign="top"> <p valign="top">业务分析师</p> <p valign="top">控制者创意</p> <p valign="top">设计者</p> <p valign="top">资源管理器</p> <p valign="top">Scrum主控</p> <p valign="top">技术作家</p> <p valign="top">Web开发人员</p> </td> 
  </tr> 
 </tbody> 
</table>

角色名称必须唯一，无法导入现有作业角色。

下表显示了要导入的用户以及每个用户的多个用户属性：

### 用户1

| **姓** | 克里斯 |
|---|---|
| **名** | 曼宁 |
| **用户名/电子邮件** | mailto:cmanning@foo.com |
| **密码** | updateMe |
| **访问权限** | 团队成员 |
| **公司** | &lt;*您的公司>* |
| **主组** | 营销 |
| **工作角色** | 业务分析师 |

{style=&quot;table-layout:auto&quot;}

### 用户2

| **姓** | Jennifer |
|---|---|
| **名** | 坎贝尔 |
| **用户名/电子邮件** | jcampbell@foo.com |
| **密码** | updateMe |
| **访问权限** | 项目经理 |
| **公司** | &lt;*您的公司>* |
| **主组** | 营销 |
| **工作角色** | 项目经理 |

{style=&quot;table-layout:auto&quot;}

### 用户3

| **姓** | 吉尔 |
|---|---|
| **名** | 沙利文 |
| **用户名/电子邮件** | jsullivan@foo.com |
| **密码** | updateMe |
| **访问权限** | 技术支持 |
| **公司** | &lt;*您的公司>* |
| **主组** | 销售 |
| **工作角色** | 销售代表 |

{style=&quot;table-layout:auto&quot;}

### 用户4

| **姓** | 马克 |
|---|---|
| **名** | 刘易斯 |
| **用户名/电子邮件** | mlewis@foo.com |
| **密码** | updateMe |
| **访问权限** | 组合管理 |
| **公司** | &lt;*您的公司>* |
| **主组** | 财务 |
| **工作角色** | 控制器 |

{style=&quot;table-layout:auto&quot;}

### 用户5

| **姓** | 帕姆 |
|---|---|
| **名** | 雷诺 |
| **用户名/电子邮件** | preynolds@foo.com |
| **密码** | updateMe |
| **访问权限** | 项目经理 |
| **公司** | *您的公司>* |
| **主组** | 营销 |
| **工作角色** | IT |

{style=&quot;table-layout:auto&quot;}

### 用户6

| **姓** | Ray |
|---|---|
| **名** | 安德鲁斯 |
| **用户名/电子邮件** | randrews@foo.com |
| **密码** | updateMe |
| **访问权限** | 管理员 |
| **公司** | *您的公司>* |
| **主组** | 资源管理器 |
| **工作角色** | 无 |

{style=&quot;table-layout:auto&quot;}

## 下载启动模板

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统** > **启动** > **导入数据。**

1. 单击 **更多选项** 查看导入选项的完整列表。
1. 选择要导入的访问级别、公司、组、作业角色和用户对象。

## 输入公司信息

1. 打开 **Workfront.xlsx** 文件。

   >[!TIP]
   >
   >使用非常宽的数据表时，您可能希望使用电子表格编辑器的冻结窗格（或等效的）工具来使电子表格更易于使用。

1. 转到“CMPY公司”表。

   除非公司已在系统中，否则此值应为空。 ![](assets/cmpysheet-350x16.png)

   ![](assets/companyid--1--350x78.png)

1. 在中指定TRUE **isNew** 列。
1. 对要添加的每个公司重复此操作。 （在此示例中，为第3-6行完成此操作，因为添加了四个公司。）

   ![](assets/cmpyisnew-350x86.png)

1. 指定唯一ID。

   必须对ID列的每行执行此操作。 从1开始的整数在创建新记录时非常有效。

   ![](assets/cmpyisnew-350x86.png)

1. 设置名称。

   在 **setName** 列。

   ![](assets/companyid-350x78.png)

1. 转到“组”(GROUP)“组”(Group)工作表。

   除非您已在Workfront中创建组，否则此工作表应仅显示每个Workfront帐户都配置的默认组。

   ![](assets/groupsheet-350x15.png) ![](assets/emptygroupsheet-350x85.png)

1. 设置 **isNew** column.Conserion将根据情景导入4个组，因此在第4行到第7行中为“isNew”列指定TRUE。
1. 指定唯一ID。

   必须对ID列的每行执行此操作。 从1开始的整数在创建新记录时非常有效。

   ![](assets/groupids-350x85.png)

1. 设置名称。

   指定 **setName** 列。

   ![](assets/groupnames-350x85.png)

   指定角色信息。 转到“角色”角色表。

1. 除非您已在帐户中创建或删除了角色，否则此工作表应显示8个已与每个Workfront帐户一起配置的角色。

   ![](assets/groupnames-350x85.png)

1. 设置True语句。

   正在导入7个作业角色，在“isNew”列的行12到18中输入TRUE。

   ![](assets/roleisnew-350x104.png)

1. 指定唯一ID。

   必须对ID列的每行执行此操作。 从1开始的整数在创建新记录时非常有效。

   ![](assets/usersheet-350x16.png)

   ![](assets/roleisnew--1--350x104.png)

1. 通过在setName列中键入每个角色的名称来提供其名称。

   ![](assets/roleisnew-350x104.png)

1. 根据需要提供其他详细信息。

   根据需要，包括您正在创建的角色的开单费率、成本费率和描述。

1. 转到“用户”用户工作表以输入“用户信息”。

   除非您已在帐户中创建用户，否则此工作表应仅显示已配置了每个Workfront帐户的管理员用户。

   ![](assets/rolenames-350x104.png) ![](assets/emptyusersheet-350x52.png)

1. 由于将导入6个用户，因此在“isNew”列的第4行到第9行中指定TRUE可设置True值。

   ![](assets/userisnew-350x52.png)

1. 通过在ID列的每行中指定唯一ID来设置唯一ID。 通常，从1开始的整数很适合用于新记录。

   ![](assets/userisnew-350x52.png)

1. 将每个用户的名称输入到“setFirstName”和“setLastName”列中。

   ![](assets/usernames-350x52.png)

1. 通过在“setEmail”、“setPassword”和“setUsername”列中指定值来设置详细信息值。

   ![](assets/usercredentials-350x52.png)

1. 指定访问级别值。

   例如，Chris Manning（团队成员）在“ACSLVL访问级别”(ACSLVL Access Level)工作表上查找团队成员访问级别的ID。 将ID复制到剪贴板，然后在“用户”工作表中，将其粘贴到 **setAccessLevelID** Chris行的列。

   为每个用户和访问级别重复此步骤。

   ![](assets/copyalid-350x171.png) ![](assets/pastealid-350x59.png)

1. 指定主组详细信息。

   根据情景，克里斯·曼宁属于营销团队。 在“群组”工作表中，找到营销群组的ID，将其复制到剪贴板，然后在“用户”工作表中，将其粘贴到 **setHomeGroupID** Chris行的列。&#x200B;对每个用户和组分配重复此步骤。

   ![](assets/copygroupid-1-350x133.png) ![](assets/pastegroupid-350x59.png)

1. 指定公司详细信息。

   此方案中的所有用户都属于同一公司。 在“CMPY公司”工作表中，找到*您自己的公司*公司的ID，将该ID复制到剪贴板，然后在“用户用户”选项卡中，将此值粘贴到“setCompanyID”列的每一行中&#x200B;。

   对每个用户和组分配重复此步骤。

   ![](assets/companyid--1--350x78.png)

   ![](assets/pastecompanyid-350x84.png)

1. 指定作业角色详细信息。

   根据情景，克里斯·曼宁将担任商业分析师。 在“角色”角色工作表中，找到Business Analyst角色的ID，将其复制到剪贴板，然后在“用户”工作表中，将其粘贴到Chris行的“setRoleID”列中。&#x200B;对每个用户和组分配重复此步骤。

   ![](assets/copyroleid-350x149.png)

   ![](assets/pasteroleid-350x95.png)

1. 根据需要填写其他用户详细信息，然后保存文件。
1. 导入Excel文件。

   按照 **导入Kick Start文件** 本文章的章节。
