---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart，kick-start，kickstarts，kick-starts
navigation-topic: use-kick-starts
title: 快速启动方案：公司、组、角色和用户快速启动准备
description: 开始实施Adobe Workfront时，您可以导入客户列表、内部部门、职位角色和用户信息，而不是手动输入数据。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: a8faf4aa1a0a1b60f61c0c981c3be1b0d9d033a4
workflow-type: tm+mt
source-wordcount: '1218'
ht-degree: 2%

---

# 快速启动方案：公司、组、角色和用户快速启动准备

开始实施Adobe Workfront时，您可以导入客户列表、内部部门、职位角色和用户信息，而不是手动输入数据。

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
   <td>
   <p> 新增：标准</p>
   或
   <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[!UICONTROL 系统管理员]</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 您可以导入的内容

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
   <td valign="top"> <p>Acme， Co</p> <p>Workfront公司</p> <p><em>您的公司</em> </p> <p>XYZ公司</p> </td> 
   <td valign="top"> <p valign="top" rowspan="7">财务</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">营销 </p> <p valign="top" rowspan="7">销售额</p> </td> 
   <td valign="top"> <p valign="top">业务分析师</p> <p valign="top">Creative控制器</p> <p valign="top">设计者</p> <p valign="top">资源管理器</p> <p valign="top">Scrum Master</p> <p valign="top">技术作者</p> <p valign="top">Web开发人员</p> </td> 
  </tr> 
 </tbody> 
</table>

角色名称必须是唯一的。 无法导入现有工作角色。

下表显示了要导入的用户以及每个用户的几个用户属性：

### 用户1

| **名字** | 克里斯 |
|---|---|
| **姓氏** | Manning |
| **用户名/电子邮件** | mailto:cmanning@foo.com |
| **密码** | 更新我 |
| **访问** | 团队成员 |
| **公司** | &lt;*您的公司>* |
| **主组** | 营销 |
| **工作角色** | 业务分析师 |

{style="table-layout:auto"}

### 用户2

| **名字** | Jennifer |
|---|---|
| **姓氏** | 坎贝尔 |
| **用户名/电子邮件** | jcampbell@foo.com |
| **密码** | 更新我 |
| **访问** | 项目经理 |
| **公司** | &lt;*您的公司>* |
| **主组** | 营销 |
| **工作角色** | 项目经理 |

{style="table-layout:auto"}

### 用户3

| **名字** | 吉尔 |
|---|---|
| **姓氏** | 沙利文 |
| **用户名/电子邮件** | jsullivan@foo.com |
| **密码** | 更新我 |
| **访问** | 技术支持 |
| **公司** | &lt;*您的公司>* |
| **主组** | 销售额 |
| **工作角色** | 销售代表 |

{style="table-layout:auto"}

### 用户4

| **名字** | 马克 |
|---|---|
| **姓氏** | 刘易斯 |
| **用户名/电子邮件** | mlewis@foo.com |
| **密码** | 更新我 |
| **访问** | 组合管理 |
| **公司** | &lt;*您的公司>* |
| **主组** | 财务 |
| **工作角色** | 控制器 |

{style="table-layout:auto"}

### 用户5

| **名字** | Pam |
|---|---|
| **姓氏** | 雷诺 |
| **用户名/电子邮件** | preynolds@foo.com |
| **密码** | 更新我 |
| **访问** | 项目经理 |
| **公司** | *您的公司>* |
| **主组** | 营销 |
| **工作角色** | IT |

{style="table-layout:auto"}

### 用户6

| **名字** | Ray |
|---|---|
| **姓氏** | Andrews |
| **用户名/电子邮件** | randrews@foo.com |
| **密码** | 更新我 |
| **访问** | 管理员 |
| **公司** | *您的公司>* |
| **主组** | 资源管理器 |
| **工作角色** | 无 |

{style="table-layout:auto"}

## 下载快速启动模板

{{step-1-to-setup}}

1. 单击&#x200B;**系统** > **Kick-Starts** > **导入数据。**

1. 单击&#x200B;**更多选项**&#x200B;查看导入选项的完整列表。
1. 选择要导入的访问级别、公司、组、工作角色和用户对象。

## 输入公司信息

1. 打开您刚刚下载的&#x200B;**Workfront.xlsx**&#x200B;文件。

   >[!TIP]
   >
   >在使用非常宽的数据表时，您可能希望使用电子表格编辑器的冻结窗格（或等效操作）工具，使电子表格更易于使用。

1. 转到“CMPY公司”表。

   除非系统中已包含公司，否则它应该为空。 ![公司表](assets/cmpysheet-350x16.png)

   ![公司ID](assets/companyid--1--350x78.png)

1. 在&#x200B;**isNew**&#x200B;列中指定TRUE。
1. 对每个要添加的公司重复此操作。 （在本例中，请为第3-6行完成此操作，因为将添加四个公司。）

   ![公司是新的](assets/cmpyisnew-350x86.png)

1. 指定唯一ID。

   必须为ID列的每一行执行此操作。 创建新记录时，从1开始的整数工作正常。

   ![公司是新的](assets/cmpyisnew-350x86.png)

1. 设置名称。

   在&#x200B;**setName**&#x200B;列中指定每个客户的名称。

   ![公司ID](assets/companyid-350x78.png)

1. 转到“组”工作表。

   除非您已在Workfront中创建了组，否则此工作表应仅显示为Workfront的每个帐户配置的默认组。

   ![组表](assets/groupsheet-350x15.png) ![空组表](assets/emptygroupsheet-350x85.png)

1. 设置&#x200B;**isNew**&#x200B;列。根据此方案，将导入4个组，因此请为“isNew”列在第4行到第7行中指定TRUE。
1. 指定唯一ID。

   必须为ID列的每一行执行此操作。 创建新记录时，从1开始的整数工作正常。

   ![组ID](assets/groupids-350x85.png)

1. 设置名称。

   在&#x200B;**setName**&#x200B;列中指定每个部门的名称。

   ![组名](assets/groupnames-350x85.png)

   指定角色信息。 转到“角色”角色表。

1. 除非您已经在帐户中创建或删除了角色，否则此工作表应显示8个使用Workfront的每个帐户配置的角色。

   ![组名](assets/groupnames-350x85.png)

1. 设置True语句。

   正在导入七个工作角色，请在“isNew”列的行12到18中输入TRUE。

   ![角色是新的](assets/roleisnew-350x104.png)

1. 指定唯一ID。

   必须为ID列的每一行执行此操作。 创建新记录时，从1开始的整数工作正常。

   ![用户表](assets/usersheet-350x16.png)

   ![角色是新的](assets/roleisnew--1--350x104.png)

1. 通过在setName列中键入每个角色来提供其名称。

   ![角色是新的](assets/roleisnew-350x104.png)

1. 根据需要提供其他详细信息。

   根据需要包括您要创建的角色的记帐费率、成本费率和描述。

1. 转到“用户”工作表以输入用户信息。

   除非您已在帐户中创建用户，否则此工作表应仅显示使用Workfront的每个帐户配置的管理员用户。

   ![角色名称](assets/rolenames-350x104.png) ![空用户表](assets/emptyusersheet-350x52.png)

1. 由于正在导入6个用户，因此在“isNew”列的第4行到第9行中指定TRUE可设置True值。

   ![用户是新用户](assets/userisnew-350x52.png)

1. 通过在ID列的每行中指定唯一ID来设置唯一ID。 通常，从1开始的整数适用于新记录。

   ![用户是新用户](assets/userisnew-350x52.png)

1. 将每个用户的名称输入到“setFirstName”和“setLastName”列中。

   ![用户名](assets/usernames-350x52.png)

1. 通过在“setEmail”、“setPassword”和“setUsername”列中指定值来设置详细信息值。

   ![用户凭据](assets/usercredentials-350x52.png)

1. 指定访问级别值。

   例如，团队成员Chris Manning在“ACSLVL访问级别”表中查找团队成员访问级别的ID。 将ID复制到剪贴板，然后在“用户”用户工作表中将其粘贴到Chris&#39;行上的&#x200B;**setAccessLevelID**&#x200B;列中。

   对每个用户和访问级别重复此步骤。

   ![复制访问级别ID](assets/copyalid-350x171.png) ![粘贴访问级别ID](assets/pastealid-350x59.png)

1. 指定主组详细信息。

   根据场景，Chris Manning属于营销组。 在“组”工作表上，找到营销组的ID，将其复制到剪贴板中，然后在“用户”工作表上将其粘贴到Chris行上的&#x200B;**setHomeGroupID**&#x200B;列中。&#x200B;AEM对每个用户和组分配重复此步骤。

   ![复制组ID](assets/copygroupid-1-350x133.png) ![粘贴组ID](assets/pastegroupid-350x59.png)

1. 指定公司详细信息。

   此方案中的所有用户属于同一公司。 在CMPY公司工作表上，找到*您自己的公司*公司的ID，将ID复制到剪贴板，然后在“用户用户”选项卡上，将此值粘贴到“setCompanyID”列的每一行中&#x200B;。

   对每个用户和组分配重复此步骤。

   ![公司ID](assets/companyid--1--350x78.png)

   ![粘贴公司ID](assets/pastecompanyid-350x84.png)

1. 指定工作角色详细信息。

   根据设想，克里斯·曼宁将担任业务分析员。 在“角色”工作表上，找到Business Analyst角色的ID，将其复制到剪贴板中，然后在“用户”工作表上将其粘贴到Chris行上的“setRoleID”列中。&#x200B;AEM对每个用户和组分配重复此步骤。

   ![复制角色ID](assets/copyroleid-350x149.png)

   ![粘贴角色ID](assets/pasteroleid-350x95.png)

1. 根据需要填写其他用户详细信息，然后保存文件。
1. 导入Excel文件。

   按照[使用快速启动模板](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)将数据导入Adobe Workfront中提供的说明进行操作。



>[!NOTE]
>
>导入到Workfront的用户创建时处于已停用和待审批状态。
> 
>如果贵组织已迁移到Adobe Admin Console，并且用户在几分钟内没有转变为“已停用”和“未决批准”状态，则您可以将该批用户直接添加到Adobe Admin Console。
>
>有关说明，请参阅[管理多个用户 | 在Adobe文档中批量CSV上传](https://helpx.adobe.com/cn/enterprise/using/bulk-upload-users.html)。
