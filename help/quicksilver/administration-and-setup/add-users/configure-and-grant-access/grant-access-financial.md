---
title: 授予对财务数据的访问权限
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以定义用户对其访问级别在Workfront中访问财务数据的权限。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# 授予对财务数据的访问权限

{{highlighted-preview}}

作为Adobe Workfront管理员，您可以通过用户的访问级别定义用户对以下内容的访问权限，如[访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述：

* Workfront中项目的财务信息
* 资源规划工具中的资源预算信息

## 访问要求

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
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 授予对财务数据的访问权限的注意事项

授予用户访问Workfront中财务数据的权限时，请考虑以下事项：

* 访问级别不允许访问财务数据的用户无法为项目创建风险。 有关详细信息，请参阅[创建和编辑项目中的风险](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)。
* 您还可以使用访问级别来确定用户可以采用哪些Resource Management活动来预算或查看资源分配。 有关信息，请参阅[授予对资源管理的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)。

## 使用自定义访问级别配置用户对财务数据的访问

1. 开始创建或编辑访问级别，如[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 单击财务数据右侧&#x200B;**查看**&#x200B;或&#x200B;**编辑**&#x200B;按钮上的齿轮图标![](assets/gear-icon-settings.png)，然后在&#x200B;**微调设置**&#x200B;下选择要授予的功能。

   ![](assets/financial-data-fine-tune-nwe.png)

1. （可选）在&#x200B;**允许**&#x200B;的管理访问权限区域，选择以下选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">汇率</td> 
      <td> <p>在Workfront中添加新货币。</p> <p>如果没有此访问权限，用户只能向其创建的项目添加现有货币。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">费用</td> 
      <td> <p>查看Workfront中对象的所有费用。</p> <p>这不允许用户创建新的费用类型。</p> <p>如果没有此访问权限，用户只能查看以下内容：</p> 
       <ul> 
        <li>他们管理的项目、任务或问题的费用</li> 
        <li>他们自己的费用</li> 
        <li>他们下属的开支</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）要为您正在处理的访问级别中的其他对象和区域配置访问设置，请继续[配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中列出的文章之一，例如[授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)。
1. 完成后，单击&#x200B;**保存**。

   创建访问级别后，可将其分配给用户。 有关详细信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 访问共享财务信息

通过授予其他用户对某个项目、任务或问题的权限，您可以与其共享该项目、任务或问题的财务信息，如[共享对象的财务权限](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md)中所述。

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

当您与其他用户共享任何对象时，收件人在该对象上的权限由以下两项共同决定：

* 您授予收件人对象的权限
* 收件人针对对象类型的访问级别设置

## 按许可证类型访问财务信息

有关每个访问级别中的用户可以如何处理财务信息的信息，请参阅[适用于每个对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)一文中的[财务数据](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia)部分。

## 通过设置访问财务信息

以下信息可帮助您了解如何使用访问级别设置来控制用户对财务数据的访问。

### 无权访问

无权访问财务数据的用户无权访问以下内容：

* 项目和任务对象下的财务部分
* 商业论证
* 记帐费率和记帐记录
* <span class="preview">费率卡</span>
* 用户偏好设置中的每小时成本和每小时计费

  您可以使用上面步骤4中“查看”按钮上的齿轮图标![](assets/gear-icon-settings.png)来配置此项。

* 工作角色的每小时成本和每小时账单

  您可以使用上面步骤4中“查看”按钮上的齿轮图标![](assets/gear-icon-settings.png)来配置此项。

### 查看访问权限

对财务数据具有“查看”权限的用户可以查看（而非编辑）以下内容：

* 项目和任务对象下的财务部分
* 商业论证
* 记帐费率和记帐记录
* 用户偏好设置中的每小时成本和每小时计费

  您可以使用上面步骤4中“查看”按钮上的齿轮图标![](assets/gear-icon-settings.png)来配置此项。

* 工作角色的每小时成本和每小时账单

  您可以使用上面步骤4中“查看”按钮上的齿轮图标![](assets/gear-icon-settings.png)来配置此项。

### 编辑访问权限

对财务数据具有“编辑”权限的用户可以查看和编辑以下内容：

* 项目和任务对象下的财务部分
* 商业论证
* 记帐费率和记帐记录
* <span class="preview">费率卡</span>
* 用户偏好设置中的每小时成本和每小时计费

  您可以使用上面步骤4中“编辑”按钮上的齿轮图标![](assets/gear-icon-settings.png)来配置此设置。

* 工作角色的每小时成本和每小时账单

  您可以使用上面步骤4中“编辑”按钮上的齿轮图标![](assets/gear-icon-settings.png)来配置此设置。
