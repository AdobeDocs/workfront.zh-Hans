---
product-area: templates
navigation-topic: templates-navigation-topic
title: 从项目创建模板
description: 将现有项目另存为模板时，可以创建模板。
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 1%

---

# 从项目创建模板

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

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对模板的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目或更高权限 </p> <p>创建模板后，您将获得该模板的管理权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 从项目创建模板

1. 转到要另存为模板的项目。
1. 单击&#x200B;**更多**&#x200B;菜单![更多图标](assets/qs-more-icon-on-an-object.png)，然后单击&#x200B;**另存为模板**。
1. 为模板指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名称</td> 
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
     <tr> 
      <td role="rowheader">自定义表单</td> 
      <td>使用下拉列表选择要附加到模板的任何自定义表单。 如果有任何自定义表单已与项目关联，则会显示这些自定义表单中的所有数据字段。<br>在一个模板中最多可以包含10个自定义表单。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**管理Forms**&#x200B;以删除或重新排序表单。 有关如何删除模板上的自定义表单并重新排序的信息，请参阅[自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md)。

   ![第一步](assets/save-as-template-first-step-350x159.png)另存为模板

1. 单击&#x200B;**下一步。**
1. 在&#x200B;**选项**&#x200B;部分中，选中要从模板中清除的任何信息旁边的复选框。

   ![另存为模板选项](assets/save-as-template-options-step-350x109.png)

1. 单击&#x200B;**下一步。**
1. 在&#x200B;**排除**&#x200B;部分中，选择要从项目中排除的任何任务。

   ![另存为模板排除](assets/save-as-template-exclude-350x205.png)

1. 单击&#x200B;**完成并保存模板。**

   您的模板现在显示在可用模板的列表中，并可附加到现有项目或用于创建新项目。

 
