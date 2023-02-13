---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 配置用户更新的首选项
description: 您可以配置首选项，当用户在对象的 [!UICONTROL 更新] 的上界。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# 配置用户更新的首选项

您可以配置首选项，以便用户在对象中添加注释时，有权访问某些功能 [!UICONTROL 更新] 的上界。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>要在系统级别执行这些步骤，您需要[!UICONTROL System Administrator]访问级别。</p><p>要为组执行这些操作，您必须是该组的经理。</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 允许用户在更新中添加图像

默认情况下，用户无法在更新中添加图像。 启用此首选项后，用户将能够在更新中附加图像。 该首选项适用于 [!DNL Workfront] 实例。

>[!NOTE]
>
>* 更新中保存的图像将计入文档存储限制。 有关信息，请参阅 [检查文档存储限制](../../../documents/managing-documents/check-document-storage.md).
>* 图像只能通过 [!UICONTROL 更新] 选项卡，且在 [!UICONTROL 文档] 选项卡。
>




1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).
1. 在左侧面板中，选择 **[!UICONTROL 界面]** > **[!UICONTROL 更新信息源]**.
1. 选择 **[!UICONTROL 首选项]** 选项卡。

   ![更新馈送的用户首选项](assets/updatefeeds-preferences-350x137.png)

1. 选择 **[!UICONTROL 允许用户在更新中添加图像]** 复选框。
1. 选择 **[!UICONTROL 保存]**.

   启用此首选项后，您可以随时禁用此首选项。 更新中已发布的任何图像都将保留在 [!UICONTROL 更新] 对象上的区域。
