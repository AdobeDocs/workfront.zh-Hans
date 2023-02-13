---
title: 设置元数据映射
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 元数据是与文档关联的描述性信息。 您可以设置 [!DNL Adobe Workfront] 将元数据包含到 [!DNL Workfront] 应用程序。
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# 设置元数据映射

元数据是与文档关联的描述性信息。 您可以设置 [!DNL Adobe Workfront] 将元数据包含到 [!DNL Workfront] 应用程序。

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
   <td> <p>你必须是 [!DNL Workfront] 管理员。 有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 关于 [!DNL Workfront] 元数据

中文档的元数据 [!DNL Workfront] 可以包括相关项目名称、任务说明或计划完成日期等信息。 As a [!DNL Workfront] 管理员，您可以配置 [!DNL Workfront] 包含从发送的文档的元数据 [!DNL Workfront] 更改为 [!DNL Workfront] 应用程序：

* [!DNL Workfront DAM]

在随文档一起发送元数据之前，您必须先指定或映射要包含的元数据。 您可以映射 [!DNL Workfront]. 设置元数据映射后，所有上传到 [!DNL Workfront] 应用程序将包含映射的元数据。

用户从 [!DNL Workfront] 至 [!DNL Workfront] 应用程序中，映射的元数据将沿文档进行传输。 而 [!DNL Workfront] 应用程序链接到 [!DNL Workfront]，对 [!DNL Workfront] 未反映在 [!DNL Workfront] 应用程序。 如果 [!DNL Workfront] 更改后，您必须将包含更新元数据的文档新版本发送到 [!DNL Workfront] 应用程序。

>[!NOTE]
>
>您只能在一个方向上映射元数据：从 [!DNL Workfront] to [!DNL Workfront DAM]. 链接到的文档的元数据 [!DNL Workfront] 从 [!DNL Workfront DAM] 无法转移到Workfront。

您可以映射相同的 [!DNL Workfront] 中的各种元数据字段 [!DNL Workfront DAM]，但您不能在其中任一应用程序中将元数据字段用于多个 [!DNL Workfront] 元数据字段。

配置多个 [!DNL Workfront] 导出到 [!DNL Workfront] 应用程序，首先在 [!DNL Workfront] 以显示对象的所有单个自定义字段。 然后，映射计算出的 [!DNL Workfront] 元数据字段的 [!DNL Workfront] 应用程序。 有关计算自定义字段的更多信息，请参阅 [将计算数据添加到自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

在映射元数据映射流程的字段之前，必须在 [!DNL Workfront]. 有关更多信息，请参阅 [配置文档集成](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## 配置 [!DNL Workfront] 发送元数据

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **[!UICONTROL 文档]** > **[!UICONTROL 元数据映射]**.

   ![](assets/metadata-mapping.png)

1. 在 **[!UICONTROL 为映射选择源字段]** 框中，开始键入要映射到的Workfront字段的名称 [!DNL Workfront DAM]，然后在列表中看到时将其选中。
1. 在 **[!UICONTROL 选择要映射的目标字段]** 框中，选择要使用选定 [!DNL Workfront] 字段。

1. 单击 **[!UICONTROL 添加映射]**.

   映射的字段显示在页面底部列出的映射字段中。

1. 重复步骤5和6，直到添加所有所需的 [!DNL Workfront] 字段及其对应的 [!DNL Workfront DAM] 字段。

## 删除映射的字段

1. 登录到 [!DNL Workfront] 作为管理员。
1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **[!UICONTROL 文档]** > **[!UICONTROL 元数据映射]**.

1. 在映射的字段列表中，选择要从元数据映射中删除的字段。
1. 单击 **[!UICONTROL 删除]**.

   不再映射指定的字段。 现在，当用户从 [!DNL Workfront] to [!DNL Workfront DAM]，则删除字段中包含的元数据不会随文档一起传输。

   在删除映射字段之前发送的文档将保留随其发送的原始元数据，包括已删除字段的元数据。
