---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 启用或禁用组织的快速发布
description: 您可以选择按月还是按季度接收新的Workfront功能。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 71ef7a50-7a9f-43c4-b67c-8d9fc722569f
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 1%

---

# 为您的组织启用或禁用快速发布

Adobe Workfront有两种发布新功能和更新的模型。 您可以选择按季度接收新功能，还是按更快的发布计划接收新功能。

这两种模型提供相同的功能和更新。 唯一的区别在于时机。

示例：

* 公司X启用了快速发布流程。 他们在8月将获得功能A，9月将获得功能B，10月将获得功能C。
* Y公司已禁用快速发布流程。 他们将在10月的季度发布中接收功能A、B和C。

>[!NOTE]
>
>* 在23.3版（2023年7月）之后购买Workfront的客户在默认情况下会启用快速发布流程，并且可以选择退出。
>* 对于在23.3版本之前购买了Workfront的客户，默认情况下会禁用快速发布流程，并且可以选择加入。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p> <p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>您必须是Workfront管理员。 </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 启用或禁用快速发布流程时的注意事项

启用或禁用快速发布流程时，请考虑以下事项：

* **启用**&#x200B;在季度中启用快速发布流程，使您的组织能够访问已发布到快速发布的功能和特性。

  例如，如果功能A在8月发布，功能B在9月发布，则在9月启用快速发布流程的任何组织都可以立即访问功能A和B。

* **正在禁用**&#x200B;快速发布过程在下个季度发布之前不会生效。

  例如，如果一家启用了快速发布的组织在8月禁用了该功能，那么他们仍将在9月收到快速发布功能，因为在10月发布下一个季度版本之前，他们不会迁移到季度版本。

## 为您的组织启用或禁用快速发布流程

要启用或禁用快速发布流程，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧导航中展开&#x200B;**系统**，然后单击&#x200B;**首选项**。
1. 要启用快速释放，请选中&#x200B;**允许快速释放进程**&#x200B;复选框。

   或

   要禁用快速发布并移至季度发布周期，请取消选中&#x200B;**允许快速发布流程**&#x200B;复选框。

1. 在弹出窗口中确认您的选择。
1. 单击&#x200B;**保存**。
