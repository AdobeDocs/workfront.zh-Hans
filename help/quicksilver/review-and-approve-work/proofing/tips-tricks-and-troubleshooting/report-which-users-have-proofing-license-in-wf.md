---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 在Adobe Workfront中列出具有验证许可证的用户
description: 您可以查看哪些用户当前在Adobe Workfront中通过下列任一方式启用了“用户可以生成验证”选项。
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# 在Adobe Workfront中列出具有验证许可证的用户

您可以查看哪些用户当前在Adobe Workfront中通过下列任一方式启用了“用户可以生成验证”选项。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>旧版计划：选择或Premium</p> <p>有关使用其他计划进行验证访问的更多信息，请参阅<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>编辑以下项的访问权限：</p> 
    <ul> 
     <li> <p>创建报告、功能板和日历</p> </li> 
     <li> <p>创建筛选器、视图和分组</p> </li> 
    </ul> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、角色或验证权限配置文件，请联系您的Workfront或Workfront Proof管理员。

## 创建用户报告

您可以创建用户报告，以查看哪些用户可以生成验证：

1. 导航到&#x200B;**报告**&#x200B;区域。
1. 单击&#x200B;**新建报表**&#x200B;下拉菜单，然后单击&#x200B;**用户报表**。

1. 在&#x200B;**筛选器**&#x200B;选项卡上，单击&#x200B;**添加筛选器规则**。

1. 在可用字段中，展开&#x200B;**用户**，然后单击&#x200B;**拥有证明许可证**。

1. 选择&#x200B;**等于** > **True**。

   ![report_proflicenses.png](assets/report-prooflicenses-350x135.png)

1. 单击&#x200B;**保存+关闭**。

   报表会显示Workfront中分配了验证许可证的所有用户。

## 更新人员视图

您可以在“人员”视图中添加新列，以查看哪些用户可以生成验证：

1. 转到&#x200B;**人员**&#x200B;区域。
1. 单击&#x200B;**人员**&#x200B;选项卡。
1. 在&#x200B;**视图**&#x200B;下拉菜单中，执行以下任一操作：

   * 若要将此信息添加到现有视图，请选择要自定义的视图，然后单击&#x200B;**自定义视图**。
   * 若要将此信息添加到新视图，请单击&#x200B;**新建视图**。

1. 单击&#x200B;**添加列**。
1. 在可用字段中，展开&#x200B;**用户**，然后单击&#x200B;**拥有证明许可证**。

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存视图**&#x200B;或&#x200B;**另存为新视图**。

   该视图显示&#x200B;**True**&#x200B;或&#x200B;**False**，具体取决于用户是否分配了验证许可证。
