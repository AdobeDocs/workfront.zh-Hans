---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 配置用户更新的首选项
description: 当用户在对象的[!UICONTROL 更新]区域中添加注释时，您可以配置用于访问某些功能的首选项。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 配置用户更新的首选项

<!--Audited: 08/2025-->

您可以配置首选项，使用户在对象的[!UICONTROL 更新]区域中添加注释时能够访问某些功能。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td><p>[！UICONTROL标准版]</p>
   <p>[！UICONTROL计划]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td><p>系统管理员，在系统级别执行这些步骤。 </p>
   <p>计划员，为组执行这些步骤，并且是该组的经理。</p></td>
  </tr> 
 </tbody> 
</table>

*有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   Or
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>To perform these steps at the system level, you need the [!UICONTROL System Administrator] access level.</p><p>To perform them for a group, you must be a manager of that group.</p></td>
  </tr> 
 </tbody> 
</table>-->

## 允许用户在更新中添加图像

默认情况下，用户无法在更新中添加图像。 启用此首选项后，用户将能够在更新中附加图像。 该首选项适用于[!DNL Workfront]实例的所有区域中的所有更新。

>[!NOTE]
>
>* 更新中保存的图像计入文档存储限制。 有关信息，请参阅[检查文档存储限制](../../../documents/managing-documents/check-document-storage.md)。
>* 可通过对象上的[!UICONTROL 更新]选项卡访问图像，也可在[!UICONTROL 主菜单]下的[!UICONTROL 文档]区域访问图像。
>

1. 单击&#x200B;**[!UICONTROL 右上角的]**&#x200B;主菜单![图标](assets/main-menu-icon.png)主菜单图标[!DNL Adobe Workfront]，然后单击&#x200B;**[!UICONTROL 设置]**![齿轮设置图标](assets/gear-icon-settings.png)。
1. 在左侧面板中，选择&#x200B;**[!UICONTROL 界面]** > **[!UICONTROL 更新源]**。
1. 选择&#x200B;**[!UICONTROL 首选项]**&#x200B;选项卡。

   ![更新源的用户首选项](assets/updatefeeds-preferences-350x137.png)

1. 选中&#x200B;**[!UICONTROL 允许用户在更新中添加图像]**&#x200B;复选框。
1. 选择&#x200B;**[!UICONTROL 保存]**。

   启用此首选项后，您可以随时将其禁用。 任何已在更新中发布的图像将保留在对象的[!UICONTROL 更新]区域中。
