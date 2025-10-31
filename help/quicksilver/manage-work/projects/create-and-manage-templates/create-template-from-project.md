---
product-area: templates
navigation-topic: templates-navigation-topic
title: 从项目创建模板
description: 将现有项目另存为模板时，可以创建模板。
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 1%

---

# 从项目创建模板

<!--Audited: 10/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

将现有项目另存为模板时，可以创建模板。

将现有项目另存为模板后，即可使用新模板创建新项目。 这简化并加快了项目创建过程。

>[!NOTE]
>
>将项目另存为模板时，没有为模板保存任务和项目的实际日期。
>
>模板及其任务没有实际日期，而是指示任务可能从哪天（从未来项目可能开始的时间）开始以及任务可能需要在哪一天完成。 使用模板创建未来项目时，项目将接收实际日期。 有关信息，请参阅[创建项目](../create-projects/create-project.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p> 
   <p>规划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对模板的访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目或更高权限 </p> <p>创建模板后，您将获得该模板的管理权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you create it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 从项目创建模板

1. 转到要另存为模板的项目。
1. 单击&#x200B;**更多**&#x200B;菜单![更多图标](assets/more-icon.png)，然后单击&#x200B;**另存为模板**。
1. 为模板指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">模板名称</td> 
      <td>指定模板的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>提供模板的描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">为活动</td> 
      <td> <p>从以下选项中选择：</p> 
       <ul> 
        <li> <p><strong>是</strong>：其他用户可以找到模板并将其附加到项目。</p> </li> 
        <li><strong>否</strong>：其他用户找不到该模板，也无法将其附加到项目。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击左侧面板中的&#x200B;**自定义Forms**。
1. 单击&#x200B;**添加自定义表单**&#x200B;字段，然后开始键入自定义项目的名称，或从列表中选择一个名称。

   如果有任何自定义表单已与项目关联，则这些自定义表单中现有字段中的所有信息将显示在表单上。

   在一个模板中最多可以包含10个自定义表单。

1. 将鼠标悬停在表单名称上，然后单击以将其拖放到新位置。

   ![将项目另存为框顶部的模板](assets/save-project-as-template-top-of-the-form.png)

1. 单击左侧面板中的&#x200B;**选项**，然后选择要传输到模板的字段或项。

   默认情况下，将选中所有项目。 取消选择的项目不会转移到模板。

   ![另存为模板选项](assets/save-project-as-template-options-area.png)

1. 单击左侧面板中的&#x200B;**排除**，然后选择要从项目中排除的任何任务。

   ![另存为模板排除](assets/save-project-as-template-exclude-area.png)

1. 单击&#x200B;**完成并保存模板。**

   您的模板现在会显示在可用模板列表中。 用户可以将新模板附加到现有项目，也可以使用它来创建项目。


