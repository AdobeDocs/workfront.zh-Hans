---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：包含校样链接的文档报告
description: “查看：包含校样链接的文档报告
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# 查看：包含校样链接的文档报告

在此文档视图中，您可以插入指向文档当前版本校样的链接。

![](assets/view-document-with-proof-link-350x92.png)

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 查看包含校样链接的文档报表

要应用此视图，请执行以下操作：

1. 转到文档列表。
1. 从 **查看** 下拉菜单，选择 **新建视图**.

1. 单击 **添加列**.
1. 单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码：

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >将“您的域”替换为实际的Workfront域。 例如，如果您公司的Workfront URL为 *Company.my.workfront.com*，则您的域为“公司”。

1. 单击 **保存**，则 **保存视图**.
1. 键入视图的名称，然后单击 **保存视图**.
1. （可选）要确保仅显示带校样的文档，请执行以下操作以添加过滤器：

   1. 单击 **过滤器** 下拉菜单，然后单击 **新建过滤器**.
   1. 单击 **添加过滤器规则** 然后开始键入校样所有者，然后选择 **校样所有者ID** 当它显示在列表中时。
   1. 选择 **不为空** （在过滤器修饰符中）。
   1. 单击 **保存过滤器**，键入过滤器的名称，然后单击 **保存过滤器**.

1. 单击校样链接列中的链接以访问文档最后一个版本的校样。
