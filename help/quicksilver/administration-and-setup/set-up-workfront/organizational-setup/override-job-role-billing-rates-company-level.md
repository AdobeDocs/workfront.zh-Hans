---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 覆盖公司级别的工作角色记帐费率
description: 创建工作角色后，您可以选择为该角色选择每小时记帐费率。 您可以创建特定于公司的每小时记帐费率。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

---

# 覆盖公司级别的工作角色记帐费率

创建工作角色后，您可以选择为该角色选择每小时记帐费率。 您可以创建特定于公司的多个小时记帐费率。 每个记帐费率在特定日期范围内有效。

在项目级别，您可以启用一个选项，以允许公司级别的记帐费率覆盖项目级别的费率。 有关更多信息，请参阅 [用公司级别的记帐费率覆盖项目级别的记帐费率](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>如果您不是系统管理员，则可以管理对公司的访问权限</p> <p>[！UICONTROL Edit]对财务数据的访问权限</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 覆盖或更改用于特定工作角色的已建立记帐费率

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe] Workfront，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 公司]**.
1. 找到分配工作角色的公司。
1. 单击列表中的公司名称。
1. 单击 **[!UICONTROL 记帐费率]** 在左侧面板中。
1. 单击 **[!UICONTROL 添加记帐费率] > [!UICONTROL 新建记帐费率]**，或选择要编辑的现有费率。
1. 在 [!UICONTROL 新建记帐费率] 对话框，选择 [!UICONTROL **工作角色**] 以定义开单费率。

   此 [!UICONTROL **默认记帐费率**] 显示此工作角色的系统级别费率。

   ![新建记帐费率对话框](assets/date-effective-billing-rates-for-company.png)

1. 在 [!DNL **记帐费率1**] 字段中，输入记帐费率。 然后，单击 [!UICONTROL **保存**] 以一次性覆盖记帐费率。

   或

   单击 [!UICONTROL **添加费率**] 以添加具有有效日期的更多记帐费率。

1. （视情况而定）如果要添加多个开单费率，请输入以下信息：

   * **[!UICONTROL 记帐费率1]、2等**：时间段的记帐费率的值。
   * **[!UICONTROL 开始日期]**：费率生效的日期。
   * **[!UICONTROL 结束日期]**：费率结束的日期。

     记帐费率1没有开始日期，最后一个记帐费率没有结束日期。 某些日期会自动添加。 例如，如果记帐费率1没有结束日期，并且您添加开始日期为2023年5月1日的记帐费率2，则结束日期为2023年4月30日将添加到记帐费率1，这样不存在间隔。

1. 单击&#x200B;[!UICONTROL **保存**]。

   >[!NOTE]
   >
   >项目上工作角色费率的更改将仅影响该项目。 公司级别的费率更改将影响所有项目。 有关更多信息，请参阅 [改写工作角色开单费率和计算项目收入概览](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
