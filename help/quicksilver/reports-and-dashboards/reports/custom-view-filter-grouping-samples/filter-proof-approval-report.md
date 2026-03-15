---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 筛选器：证明批准报告以省略以前的证明版本
description: 在校样批准报告上，您可以使用“当前文档版本”过滤器仅包括等待您批准的校样的当前版本。
author: Courtney
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 4%

---

# 筛选器：证明批准报告以省略以前的证明版本

<!--Audited: 10/2024-->

在校样批准报告上，您可以使用&#x200B;**为当前文档版本**&#x200B;筛选器仅包含等待您批准的校样的当前版本。

这很有用，例如，当要求您批准具有多个版本的验证时。 当您使用“是当前文档版本”过滤器运行校样审批报告时，该报告仅列出等待您审批的每个校样的当前版本，而忽略您不再需要处理的早期版本。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>投稿人或请求修改筛选器 </p>
   <p>标准或计划修改报告</p>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑报表、仪表板、日历的访问权限以修改报表</p> <p>编辑对筛选器、视图和分组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中的信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 筛选证明批准报告以省略以前的证明版本

您可以为校样批准报告创建过滤器。

1. 如果您已有证明批准报告，请将其打开。

   或

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   若要创建您自己的校样批准报告，请单击右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)或左上角的&#x200B;**主菜单**&#x200B;图标![主菜单行](assets/lines-main-menu.png)（如果可用），然后单击&#x200B;**报告** ![报告图标](assets/reports-in-main-menu.png)。

1. 单击&#x200B;**新建报告**。 此时会显示对象类型列表。
1. 单击列表中的&#x200B;**校对审批**。
此时将打开Report Builder。
1. 单击&#x200B;**筛选器**，然后单击&#x200B;**添加筛选器规则**。

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. 在&#x200B;**为报告设置筛选规则**&#x200B;框内单击，然后从列表中选择&#x200B;**校样审批**。
1. 在&#x200B;**校样审批**&#x200B;对象下的列表中单击&#x200B;**当前文档版本**。
1. 为您的滤镜修改量选择“等于”，然后选择“真”。
1. 单击Adobe Workfront左下角的&#x200B;**保存+关闭**，然后在显示的框中单击&#x200B;**应用**。

   “证明审批”报告仅显示与任何文档的当前版本关联的证明（如果任何证明审批与此筛选条件匹配）。
