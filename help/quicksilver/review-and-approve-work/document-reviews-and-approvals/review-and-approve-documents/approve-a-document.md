---
product-area: projects
navigation-topic: approvals
title: 在Workfront中批准文档
description: 如果您被指定为文档的审批者，则可通过多种方式作出审批决策。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 5490973b-99a7-4790-9d89-bf8f16ff5765
source-git-commit: 50a38ad915b639bf742a4b1f18bcb4da88e07d63
workflow-type: tm+mt
source-wordcount: '1067'
ht-degree: 0%

---

# 在Workfront中批准文档

如果您被指定为文档的审批者，则可通过多种方式作出审批决策。

有关创建新文档审批的信息，请参阅 [创建文档审阅或审批请求](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>本文内容介绍更新的文档审批功能，该功能仅适用于特定帐户。 有关标准审批流程的信息，请参阅中列出的文章 [工作审批](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

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
   <td> <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限访问与审批关联的对象</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看与审批关联的对象的权限或更高的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 从主页审批文档

1. 单击 **主页** 图标 ![](../assets/home-icon-30x29.png) 在Adobe Workfront的左上角。

   >[!NOTE]
   >
   >您的Workfront管理员可以对环境中的主页图标进行以下更改：
   >
   >* 请将其替换为用于说明贵组织的自定义图像。 在这种情况下，图标的外观将与本文中显示的有所不同。
   >
   >* 将链接到该页面的页面替换为其他页面。 在此例中，单击 **主菜单** ![](../assets/main-menu-icon.png) （位于页面的右上角），然后单击 **主页**.

1. 单击 **过滤器** ，并确保 **审批** 已选中。

   需要您批准的所有工作项都将显示在列表中。

   >[!NOTE]
   >
   >分配给工作角色或组的审批未列在主页中。 分配给团队的审批显示在工作列表的团队请求分组中。

1. 单击要为其作出批准决策的列表中的文档批准。 有关批准的信息将显示在页面的右侧。

1. 单击页面右上角的以下两个批准选项之一：

   * 此 **批准** 下拉列表包含两个选项：

      * **批准** 表示不需要对此版本的文档进行更改，并且已获得批准。

      * **批准，但有更改** 表示文档上仍需要一些细微的更改，但在进行这些更改的情况下会获得批准。 如果选择此选项，将显示一个窗口，其中包含名为的文本框 **后续步骤** 您可以在此处指定要批准文档所需的更改。 您可以输入该信息并单击 **添加消息**，或者您可以单击 **跳过** 发送批准决定，而不提供更多信息。

   * **需要工作** 表示文档版本未获得批准，需要进行重大更改。

   在主页中查看文档审批时，请考虑以下事项：

   * 请求审批的用户的名称显示在主页文档名称上方，文本为&quot;*用户A* 希望您批准……”，以及 **提交者** ，该页面位于选择批准后右侧显示的批准信息中。

   * 作出批准决策后，批准将保留在“我的批准”选项卡中，并带有文本“已作出决定”，直到您单击 **刷新** 按钮，或者直到刷新浏览器页面为止。

## 批准文档页面中的文档

1. 通过单击文档名称转到文档页面。

1. 在文档名称旁边的版本下拉列表中选择待审批的文档版本。 默认情况下将选择最新版本。

   如果当前所选文档版本具有待定的批准，则页面右上角将显示批准决策按钮；如果文档的其他版本具有待定的批准，则版本下拉菜单将显示一个红点。

   <!--
   ![](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. 单击页面右上角的以下两个批准选项之一：

   * 此 **批准** 下拉列表包含两个选项：

      * **批准** 表示不需要对此版本的文档进行更改，并且已获得批准。

      * **批准，但有更改** 表示文档上仍需要一些细微的更改，但在进行这些更改的情况下会获得批准。 如果选择此选项，将显示一个窗口，其中包含名为的文本框 **后续步骤** 您可以在此处指定要批准文档所需的更改。 您可以输入该信息并单击 **添加消息**，或者您可以单击 **跳过** 发送批准决定，而不提供更多信息。

   * **需要工作** 表示文档版本未获得批准，需要进行重大更改。

## 从“文档摘要”窗格审批文档

1. 转到包含文档的项目、任务或问题，然后选择 **文档**.

1. 单击需要您审批的文档，此时将打开“文档摘要”窗格。

1. 在版本下拉列表中选择要查看的文档版本。 默认情况下将选择最新版本。

   如果当前所选文档版本有待批准的文档，则批准决策按钮将显示在“文档摘要”窗格的右上角；如果文档的其他版本有待批准的文档，则版本下拉菜单将显示一个红点。

   <!--
   ![](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. 单击“文档摘要”窗格右上角的以下两个审批选项之一：

   * 此 **批准** 下拉列表包含两个选项：

      * **批准** 表示不需要对此版本的文档进行更改，并且已获得批准。

      * **批准，但有更改** 表示文档上仍需要一些细微的更改，但在进行这些更改的情况下会获得批准。 如果选择此选项，将显示一个窗口，其中包含名为的文本框 **后续步骤** 您可以在此处指定要批准文档所需的更改。 您可以输入该信息并单击 **添加消息**，或者您可以单击 **跳过** 发送批准决定，而不提供更多信息。

   * **需要工作** 表示文档版本未获得批准，需要进行重大更改。