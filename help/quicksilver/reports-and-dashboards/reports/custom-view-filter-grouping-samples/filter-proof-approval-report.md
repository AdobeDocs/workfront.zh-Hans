---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: “过滤器：校样批准报表以忽略以前的校样版本
description: 在校样批准报表中，您可以使用“为当前文档版本”过滤器仅包含等待批准的当前版本校样。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# 过滤器：校样批准报表可忽略以前的校样版本

在校样批准报表中，您可以使用 **是当前文档版本** 过滤器，仅包含等待您批准的校样的当前版本。

例如，如果您被要求批准具有多个版本的校样，则此功能非常有用。 在使用“为当前文档版本”过滤器运行校样批准报表时，该报表仅列出每个校样的当前版本，等待您批准，而省略了您不再需要处理的早期版本。 

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

## 过滤校样批准报表可忽略以前的校样版本

1. 如果您已经有校样批准报表，请将其打开。

   或

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   要创建自己的校样批准报告，请单击主菜单 ![](assets/main-menu-icon.png)，然后单击 **报表** ![](assets/reports-in-main-menu.png). 单击 **新建报表**. 在显示的列表中，滚动到并单击 **校样批准**. 单击 **保存并关闭**，键入 **报表名称** （可选），然后单击 **保存报表**.

1. 单击 **报表操作>编辑**.
1. 单击 **过滤器**，然后单击 **添加过滤器规则**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. 单击 **校样批准**.
1. 在显示的列表中，单击 **是当前文档版本**.
1. 单击 **保存并关闭** 在Adobe Workfront的左下角，单击 **保存报表** 框中。
