---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: 管理费率卡
description: 费率卡允许您根据位置为每个角色定义多个计费费率。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# 管理费率卡

{{highlighted-preview-article-level}}

费率卡允许您根据位置为每个角色定义多个计费费率。 您可以让位于巴黎的Designer和位于纽约的第二个Designer担任工作角色，每个角色具有不同的计费率。 但是，费率卡上的工作角色不需要位置。 费率卡上工作角色（以及可能的地点）的计费费率还可以包括有效日期。

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
   <td><p>新计划： [！UICONTROL Standard] </p>
       <p>或</p> 
       <p>当前计划： [！UICONTROL计划] </p>
   </td>    
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对[！UICONTROL财务数据]的访问权限</p> <p><b>注意</b>：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>要编辑与您共享的费率卡，您必须拥有费率卡的管理权限。</td> 
  </tr> 
 </tbody> 
</table>

+++

## 添加费率卡

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;[!UICONTROL **费率卡**]。
1. 单击&#x200B;[!UICONTROL **新建费率卡**]，然后在[!UICONTROL 新建费率卡]框中键入费率卡的名称，以替换“无标题的费率卡”。
1. （可选）在费率卡详细信息屏幕上，添加&#x200B;[!UICONTROL **描述**]。
1. （可选）要将自定义表单附加到费率卡，请单击右上角的&#x200B;[!UICONTROL **添加自定义表单**]&#x200B;字段，然后从显示的列表中选择自定义表单。

   有关附加自定义表单的详细信息，请参阅[将自定义表单添加到对象](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

1. 在左侧导航面板中单击&#x200B;[!UICONTROL **工作角色和费率**]。
1. 在“费率卡工作角色和费率”屏幕上，单击&#x200B;[!UICONTROL **添加工作角色**]。
1. 在对话框中，选择要为其定义记帐费率的&#x200B;[!UICONTROL **工作角色**]。

   默认开单费率显示此工作角色的系统层费率（如果已定义）。

   ![新建记帐费率对话框](assets/location-rate-for-rate-card.png)

1. 为工作角色选择&#x200B;[!UICONTROL **货币**]。
1. （可选）为工作角色选择&#x200B;[!UICONTROL **位置**]。
1. 在&#x200B;[!UICONTROL **记帐费率1**]&#x200B;字段中输入此位置的记帐费率。 然后，单击&#x200B;[!UICONTROL **保存**]&#x200B;以一次性覆盖记帐费率。

   或

   单击&#x200B;[!UICONTROL **添加费率**]&#x200B;以添加更多具有有效日期的特定于位置的记帐费率。

1. （视情况而定）如果要为此地点添加多个开单费率，请输入以下信息：

   * **[!UICONTROL 记帐费率1]、2等：**&#x200B;时间段的记帐费率值。
   * **[!UICONTROL 开始日期]：**&#x200B;费率覆盖开始的日期。
   * **[!UICONTROL 结束日期]：**&#x200B;费率覆盖结束的日期。

     记帐费率1没有开始日期，最后一个记帐费率没有结束日期。 某些日期会自动添加。 例如，如果记帐费率1没有结束日期，并且您添加开始日期为2023年5月1日的记帐费率2，则结束日期为2023年4月30日将添加到记帐费率1，这样不存在间隔。

1. 单击&#x200B;[!UICONTROL **保存**]。
1. （可选）要为其他位置的同一工作角色或单独的工作角色添加其他记帐费率，请单击&#x200B;[!UICONTROL **添加工作角色**]。
1. （可选）要编辑费率卡，请在“设置”的“费率卡”列表中单击费率卡的名称。 要编辑记帐费率，请单击费率卡左侧导航面板中的&#x200B;[!UICONTROL **工作角色和费率**]。 然后，选择费率并单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。

## 复制费率卡

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;[!UICONTROL **费率卡**]。
1. 选中列表中费率卡旁边的复选框，然后单击&#x200B;**复制**&#x200B;图标![复制图标](assets/copy-icon.png)。
1. 在[!UICONTROL 复制费率卡]框中键入费率卡的名称，以替换“无标题费率卡”。 然后，单击&#x200B;**保存**。

   已保存新的费率卡。 根据需要编辑费率卡详细信息、工作角色和费率。

## 删除整个费率卡

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;[!UICONTROL **费率卡**]。
1. 选中列表中费率卡旁边的复选框，然后单击&#x200B;**删除**&#x200B;图标![删除图标](assets/delete.png)。

   >[!NOTE]
   >
   >附加到项目的费率卡将从项目中删除。
