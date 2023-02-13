---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 停用或重新激活公司
description: 您可以停用不再使用的公司，同时保留其所有关联的历史数据。 如果您停用系统中某个位置已在使用的公司，则它会继续像往常一样正常运行。 不会删除或阻止。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# 停用或重新激活公司

您可以停用不再使用的公司，同时保留其所有关联的历史数据。 如果您停用系统中某个位置已在使用的公司，则它会继续像往常一样正常运行。 不会删除或阻止。

## 访问要求

要在 [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] 计划*</p> </td> 
   <td>[!UICONTROL Team]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 许可证*</p> </td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>访问级别配置*</strong> </td> 
   <td> <p>以下任一项：</p> 
    <ul> 
     <li> <p>[!UICONTROL系统管理员]访问级别，允许您编辑系统中的任何公司。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>. </p> </li> 
     <li> <p>对管理公司的管理访问权限，用于编辑系统中的任何公司。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </li> 
    </ul> <p><b>注释</b>:  
     <ul> 
      <li> <p>您还可以管理与任何分配为群组管理员的群组关联的公司。</p> </li> 
      <li> <p>要在 [!DNL Workfront] 系统时，您必须具有以下一项：</p> 
       <ul> 
        <li> <p>[!UICONTROL系统管理员]访问级别。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>. </p> </li> 
        <li> <p>在访问级别中，必须为[!UICONTROL Users]设置选择[!UICONTROL Edit]。 此外，对于[!UICONTROL用户]设置，在[!UICONTROL微调您的设置]下 <img src="assets/gear-icon-in-access-levels.png"> ，则必须启用[!UICONTROL创建]选项和两个[!UICONTROL用户管理员]选项中的至少一个选项。 </p> <p> <img src="assets/access-req-users.png" style="width: 350;height: 101;"> </p> <p>如果您使用[!UICONTROL用户管理员（群组用户）]选项，则您必须是用户所属群组的群组管理员。</p> </li> 
       </ul> <p>有关访问级别中“用户”设置的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请联系您的 [!DNL Workfront] 管理员。

## 停用或重新激活公司

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe] Workfront，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **[!UICONTROL 公司]** ![](assets/companies-icon-left-panel.png).

1. 选择一个或多个要停用或重新激活的公司。
1. 单击 **[!UICONTROL 编辑]**.
1. 对于单个公司，请禁用 **[!UICONTROL 处于活动状态]** 选项将其停用，或启用选项以将其激活。

   或

   对于多个公司，请选择 **[!UICONTROL 否]** 从 **[!UICONTROL 处于活动状态]** 下拉菜单以取消激活它们，或者 **[!UICONTROL 是]** 来激活它们。

1. 单击 **[!UICONTROL 保存更改]**.
