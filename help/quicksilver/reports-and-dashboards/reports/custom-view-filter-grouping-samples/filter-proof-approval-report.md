---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '过滤器：验证审批报告，忽略以前的验证版本'
description: 在验证审批报表中，您可以使用当前文档版本过滤器仅包括等待您审批的当前版本的验证。
author: Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# 过滤器：验证审批报告，以忽略以前的验证版本

<!--Audited: 10/2024-->

在验证审批报告中，您可以使用&#x200B;**当前文档版本**&#x200B;筛选器以仅包含等待您审批的当前版本的验证。

这很有用，例如，当要求您批准具有多个版本的验证时。 当使用当前文档版本过滤器运行验证审批报告时，该报告仅列出等待您审批的每个验证的当前版本，并忽略您不再需要处理的早期版本。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改过滤器的参与者 </p></li>
   <li><p>用于修改报告的标准</p></li> </ul>

<p>当前：</p>
   <ul><li><p>请求修改筛选器 </p></li>
   <li><p>计划修改报告</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 筛选验证审批报告以忽略以前的验证版本

您可以为验证审批报告创建过滤器。

1. 如果您已有验证审批报告，请打开它。

   或

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   要创建您自己的验证审批报告，请单击右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)或左上角的&#x200B;**主菜单**&#x200B;图标![](assets/lines-main-menu.png)（如果可用），然后单击&#x200B;**报告** ![](assets/reports-in-main-menu.png)。

1. 单击&#x200B;**新建报告**。 此时将显示对象类型列表。
1. 单击列表中的&#x200B;**校对审批**。
此时将打开Report Builder。
1. 单击&#x200B;**筛选器**，然后单击&#x200B;**添加筛选器规则**。

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. 单击报告&#x200B;**设置过滤规则**&#x200B;框中的，然后从列表中选择&#x200B;**校对审批**。
1. 单击&#x200B;**校对审批**&#x200B;对象下的列表中的&#x200B;**是当前文档版本**。
1. 为筛选器修饰符选择“等于”，然后选择“真”。
1. 单击Adobe Workfront左下角的&#x200B;**保存+关闭**，然后在显示的框中单击&#x200B;**应用**。

   验证审批报告仅显示与任何文档的当前版本关联的验证（如果任何验证审批与此筛选条件匹配）。
