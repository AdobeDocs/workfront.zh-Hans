---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '过滤器：验证审批报告，忽略以前的验证版本'
description: 在验证审批报表中，您可以使用当前文档版本过滤器仅包括等待您审批的当前版本的验证。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 过滤器：验证审批报告，以忽略以前的验证版本

在验证审批报告中，您可以使用&#x200B;**当前文档版本**&#x200B;筛选器以仅包含等待您审批的当前版本的验证。

这很有用，例如，当要求您批准具有多个版本的验证时。 当使用当前文档版本过滤器运行验证审批报告时，该报告仅列出等待您审批的每个验证的当前版本，并忽略您不再需要处理的早期版本。 

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
   <td> <p>请求修改筛选器 </p>
   <p>计划修改报告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改筛选器</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 筛选验证审批报告以忽略以前的验证版本

1. 如果您已有验证审批报告，请打开它。

   或

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   要创建您自己的验证审批报告，请单击主菜单![](assets/main-menu-icon.png)，然后单击&#x200B;**报告** ![](assets/reports-in-main-menu.png)。 单击&#x200B;**新建报告**。 在显示的列表中，滚动到&#x200B;**验证审批**&#x200B;并单击。 单击&#x200B;**保存+关闭**，键入&#x200B;**报告名称**（可选），然后单击&#x200B;**保存报告**。

1. 单击&#x200B;**报告操作>编辑**。
1. 单击&#x200B;**筛选器**，然后单击&#x200B;**添加筛选器规则**。

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. 单击&#x200B;**校对审批**。
1. 在显示的列表中，单击&#x200B;**当前文档版本**。
1. 单击Adobe Workfront左下角的&#x200B;**保存+关闭**，然后在显示的框中单击&#x200B;**保存报告**。
