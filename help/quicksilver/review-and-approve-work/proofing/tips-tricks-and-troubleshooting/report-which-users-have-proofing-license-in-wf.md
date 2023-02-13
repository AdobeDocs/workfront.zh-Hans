---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 在Adobe Workfront中列出具有校对许可证的用户
description: 您可以通过以下任一方式查看Adobe Workfront中当前启用了选项“用户可以生成校样”的用户。
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# 在Adobe Workfront中列出具有校对许可证的用户

您可以通过以下任一方式查看Adobe Workfront中当前启用了选项“用户可以生成校样”的用户。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>旧版计划：选择或Premium</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>编辑对以下项的访问权限：</p> 
    <ul> 
     <li> <p>创建报表、功能板和日历</p> </li> 
     <li> <p>创建过滤器、视图和分组</p> </li> 
    </ul> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 创建用户报表

您可以创建用户报表以查看哪些用户可以生成校样：

1. 导航到 **报表** 的上界。
1. 单击 **新建报表** 下拉菜单，然后单击 **用户报表**.

1. 在 **过滤器** ，单击 **添加过滤器规则**.

1. 在可用字段中，展开 **用户**，然后单击 **拥有校样许可证**.

1. 选择 **等于** > **True**.

   ![report_proflicenses.png](assets/report-prooflicenses-350x135.png)

1. 单击 **保存并关闭**.

   报表会显示Workfront中为其分配了校样许可证的所有用户。

## 更新“人员”视图

您可以在“人员”视图中添加新列，以查看哪些用户可以生成校样：

1. 转到 **人员** 的上界。
1. 单击 **人员** 选项卡。
1. 在 **查看** 下拉菜单中，执行以下任一操作：

   * 要将此信息添加到现有视图，请选择要自定义的视图，然后单击 **自定义视图**.
   * 要将此信息添加到新视图，请单击 **新建视图**.

1. 单击 **添加列**.
1. 在可用字段中，展开 **用户**，然后单击 **拥有校样许可证**.

1. 单击 **完成**，然后单击 **保存视图** 或 **另存为新视图**.

   此时将显示视图 **True** 或 **False** 取决于用户是否为其分配了校样许可证。
