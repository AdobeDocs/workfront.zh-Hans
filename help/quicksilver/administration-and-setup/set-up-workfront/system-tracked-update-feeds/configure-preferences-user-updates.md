---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 配置用户更新的首选项
description: 您可以配置首选项，以便在用户在对象的 [!UICONTROL 更新] 区域。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: fd876089c964d57224452023b4656cd6df40b5a3
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# 配置用户更新的首选项

您可以配置首选项，使用户在对象的 [!UICONTROL 更新] 区域。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[！UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>要在系统级别执行这些步骤，您需要[！UICONTROL系统管理员]访问级别。</p><p>要为组执行这些操作，您必须是该组的经理。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 允许用户在更新中添加图像

默认情况下，用户无法在更新中添加图像。 启用此首选项后，用户将能够在更新中附加图像。 该首选项适用于您所有区域的所有更新 [!DNL Workfront] 实例。

>[!NOTE]
>
>* 更新中保存的图像计入文档存储限制。 有关信息，请参阅 [检查文档存储限制](../../../documents/managing-documents/check-document-storage.md).
>* 图像可通过以下方式访问： [!UICONTROL 更新] 选项卡上，并且也可在 [!UICONTROL 文档] 下的区域 [!UICONTROL 主菜单].
>

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).
1. 在左侧面板中，选择 **[!UICONTROL 界面]** > **[!UICONTROL 更新信息源]**.
1. 选择 **[!UICONTROL 偏好设置]** 选项卡。

   ![更新源的用户首选项](assets/updatefeeds-preferences-350x137.png)

1. 选择 **[!UICONTROL 允许用户在更新中添加图像]** 复选框。
1. 选择 **[!UICONTROL 保存]**.

   启用此首选项后，您可以随时将其禁用。 任何已在更新中发布的图像将保留在 [!UICONTROL 更新] 对象上的区域。
