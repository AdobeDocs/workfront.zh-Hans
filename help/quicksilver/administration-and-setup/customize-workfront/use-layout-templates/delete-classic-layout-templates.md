---
title: 删除经典布局模板
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 经典Workfront Experience中的布局模板在Workfront界面中不再可用，但仍可能会影响Workfront数据。 这可能会导致报表或功能板中受布局模板（例如“共享对象”）影响的字段不一致。
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: c68b63230b07ea8c8475b710e256b5e0f049b1eb
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# 授予对布局模板的管理访问权限

经典Workfront Experience中的布局模板在Workfront界面中不再可用，但仍可能会影响Workfront数据。 这可能会导致报表或功能板中受布局模板（例如“共享对象”）影响的字段不一致。

您可以通过删除传统布局模板来解决这些不一致问题。 由于它们在Workfront界面中不可用，因此使用必须使用Workfront API来删除它们。

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
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问级别。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用API调用删除经典布局模板

您可以在浏览器的URL栏中输入API调用，然后按Enter。 API响应会显示在您的浏览器中。

>[!NOTE]
>
>无法删除全局和系统布局模板。

1. 登录到Workfront。
1. 使用以下API调用找到要删除的布局模板：
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. 记下要删除的布局模板的ID。
1. 使用以下API调用找到您的会话ID：
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >切勿与任何人共享您的会话ID。

1. 将布局模板ID和会话ID插入以下API调用：
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. 将步骤4中的API调用粘贴到浏览器的URL栏中，然后按Enter。

   这将删除布局模板。



