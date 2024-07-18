---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：文档报告，带有指向验证的链接'
description: '查看：文档报告，带有指向验证的链接'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 查看：文档报告，带有指向验证的链接

在此文档视图中，您可以插入指向文档当前版本的验证的链接。

![](assets/view-document-with-proof-link-350x92.png)

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求修改视图 </p>
   <p>计划修改报告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 查看文档报告，其中包含指向验证的链接

要应用此视图，请执行以下操作：

1. 转到文档列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 单击&#x200B;**添加列**。
1. 单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >将“您的域”替换为您的实际Workfront域。 例如，如果贵公司的Workfront URL是&#x200B;*Company.my.workfront.com*，则您的域是“公司”。

1. 单击&#x200B;**保存**，然后单击&#x200B;**保存视图**。
1. 键入视图的名称，然后单击&#x200B;**保存视图**。
1. （可选）要确保只显示带验证的文档，请执行以下操作来添加过滤器：

   1. 单击&#x200B;**筛选器**&#x200B;下拉菜单，然后单击&#x200B;**新建筛选器**。
   1. 单击&#x200B;**添加筛选规则**&#x200B;并开始键入校对所有者，然后在列表中显示&#x200B;**校对所有者ID**&#x200B;时将其选定。
   1. 为筛选器修饰符选择&#x200B;**Is Not Blank**。
   1. 单击&#x200B;**保存筛选器**，键入筛选器名称，然后单击&#x200B;**保存筛选器**。

1. 单击验证链接列中的链接可访问文档最新版本的验证。
