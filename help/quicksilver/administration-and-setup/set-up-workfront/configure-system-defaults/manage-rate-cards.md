---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: 管理费率卡
description: 费率卡允许您根据位置为每个角色定义多个计费费率。
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 961e0451ce9011a8a9f511d7d5da99368d22d6fb
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 0%

---

# 管理费率卡

{{highlighted-preview-article-level}}

费率卡允许您根据位置为每个角色定义多个计费费率。 您的工作角色可以是巴黎的设计师，也可以是纽约的第二名设计师，每个设计师的计费率各不相同。 但是，费率卡上的工作角色不需要位置。 费率卡上工作角色（以及可能的地点）的计费费率还可以包括有效日期。

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
   <td><p>旧版计划： [！UICONTROL计划]</p>
       <p>当前计划： [！UICONTROL Standard]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对[！UICONTROL财务数据]的访问权限</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>要编辑与您共享的费率卡，您必须拥有费率卡的管理权限。</td> 
  </tr> 
 </tbody> 
</table>

## 添加费率卡

{{step-1-to-setup}}

1. 在左侧面板中，单击 [!UICONTROL **费率卡**].
1. 单击 [!UICONTROL **新建费率卡**]，然后在中输入费率卡的名称 [!UICONTROL **费率卡**] 字段，以替换“无标题费率卡”。
1. 在信息卡屏幕上，单击 [!UICONTROL **添加工作角色**].
1. 在对话框中，选择 [!UICONTROL **工作角色**] 以定义开单费率。

   默认开单费率显示此工作角色的系统层费率（如果已定义）。

   ![新建记帐费率对话框](assets/location-rate-for-rate-card.png)

1. 选择 [!UICONTROL **货币**] 工作角色的。
1. （可选）选择 [!UICONTROL **位置**] 工作角色的。
1. 在 [!UICONTROL **记帐费率1**] 字段中，输入此位置的记帐费率。 然后，单击 [!UICONTROL **保存**] 以一次性覆盖记帐费率。

   或

   单击 [!UICONTROL **添加费率**] 以添加更多具有有效日期的特定于位置的记帐费率。

1. （视情况而定）如果要为此地点添加多个开单费率，请输入以下信息：

   * **[!UICONTROL 记帐费率1]、2等：** 时间期间的记帐费率的值。
   * **[!UICONTROL 开始日期]：** 费率覆盖开始的日期。
   * **[!UICONTROL 结束日期]：** 费率覆盖结束的日期。

     记帐费率1没有开始日期，最后一个记帐费率没有结束日期。 某些日期会自动添加。 例如，如果记帐费率1没有结束日期，并且您添加开始日期为2023年5月1日的记帐费率2，则结束日期为2023年4月30日将添加到记帐费率1，这样不存在间隔。

1. 单击&#x200B;[!UICONTROL **保存**]。
1. （可选）要为其他位置的同一工作角色或单独的工作角色添加其他记帐费率，请单击 [!UICONTROL **添加工作角色**].
1. （可选）要编辑记帐费率，请在费率卡中选择该费率，然后单击 **编辑** 图标。

## 复制费率卡

{{step-1-to-setup}}

1. 在左侧面板中，单击 [!UICONTROL **费率卡**].
1. 选中列表中费率卡旁边的复选框，然后单击 **复制** 图标 ![“复制”图标](assets/copy-icon.png).

   添加了重复速率卡片。 单击列表中的费率卡名称以更改其名称。

## 删除整个费率卡

{{step-1-to-setup}}

1. 在左侧面板中，单击 [!UICONTROL **费率卡**].
1. 选中列表中费率卡旁边的复选框，然后单击 **删除** 图标 ![“删除”图标](assets/delete.png).

   >[!NOTE]
   >
   >附加到项目的费率卡将从项目中删除。
