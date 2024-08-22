---
title: 设置元数据映射
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 元数据是与文档关联的描述性信息。 您可以设置 [!DNL Adobe Workfront] 以包含发送至 [!DNL Workfront] 应用程序的文档的元数据。
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# 设置元数据映射

元数据是与文档关联的描述性信息。 您可以设置[!DNL Adobe Workfront]以包含发送至[!DNL Workfront]应用程序的文档的元数据。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td> <p>您必须是[!DNL Workfront]管理员。 有关详细信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> <p><b>注意</b>：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 关于[!DNL Workfront]元数据

[!DNL Workfront]中文档的元数据可能包含相关项目名称、任务描述或计划完成日期等信息。 作为[!DNL Workfront]管理员，您可以将[!DNL Workfront]配置为包含元数据，其中包含从[!DNL Workfront]发送到以下[!DNL Workfront]应用程序的文档：

* [!DNL Workfront DAM]

必须先指定或映射要包含的元数据，然后才能随文档发送元数据。 您可以映射[!DNL Workfront]中使用的任何字段。 设置元数据映射后，上载到[!DNL Workfront]应用程序的所有文档都将包含映射的元数据。

当用户将文档从[!DNL Workfront]发送到[!DNL Workfront]应用程序时，映射的元数据将随文档一起传输。 尽管[!DNL Workfront]应用程序中的文档版本链接到[!DNL Workfront]，但在[!DNL Workfront]中对文档元数据所做的更改未反映在[!DNL Workfront]应用程序中的文档元数据中。 如果[!DNL Workfront]中的映射字段已更改，则必须将包含更新元数据的文档的新版本发送到[!DNL Workfront]应用程序。

>[!NOTE]
>
>只能在一个方向上映射元数据：从[!DNL Workfront]到[!DNL Workfront DAM]。 无法将从[!DNL Workfront DAM]链接到[!DNL Workfront]的文档的元数据传输到Workfront。

您可以将同一[!DNL Workfront]字段映射到[!DNL Workfront DAM]中的各种元数据字段，但是不能在其中任一应用程序中对多个[!DNL Workfront]元数据字段使用元数据字段。

要将多个[!DNL Workfront]字段配置为导出到[!DNL Workfront]应用程序中的一个元数据字段，请先在[!DNL Workfront]中创建计算自定义字段以显示对象的所有单个自定义字段。 然后，将计算的[!DNL Workfront]字段映射到[!DNL Workfront]应用程序中的元数据字段。 有关计算自定义字段的详细信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

在为元数据映射进程映射字段之前，必须在[!DNL Workfront]中启用该应用程序。 有关详细信息，请参阅[配置文档集成](../../administration-and-setup/configure-integrations/configure-document-integrations.md)。

## 配置[!DNL Workfront]以发送元数据

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 文档]** > **[!UICONTROL 元数据映射]**。

   ![](assets/metadata-mapping.png)

1. 在&#x200B;**[!UICONTROL 选择要映射的Source字段]**&#x200B;框中，开始输入要映射到[!DNL Workfront DAM]的Workfront字段的名称，然后在列表中看到该字段时将其选定。
1. 在&#x200B;**[!UICONTROL 选择要映射的目标字段]**&#x200B;框中，选择要使用选定[!DNL Workfront]字段中的信息填充的字段。

1. 单击&#x200B;**[!UICONTROL 添加映射]**。

   映射的字段显示在页面底部列出的映射字段中。

1. 重复步骤5和6，直到您添加所有所需的[!DNL Workfront]字段及其对应的[!DNL Workfront DAM]字段。

## 删除映射字段

1. 以管理员身份登录到[!DNL Workfront]。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 文档]** > **[!UICONTROL 元数据映射]**。

1. 在映射的字段列表中，选择要从元数据映射中删除的字段。
1. 单击&#x200B;**[!UICONTROL 删除]**。

   指定的字段不再映射。 现在，当用户将文档从[!DNL Workfront]发送到[!DNL Workfront DAM]时，已删除字段中包含的元数据未随文档一起传输。

   在您删除映射字段之前发送的文档会保留随其发送的原始元数据，包括已删除字段的元数据。
