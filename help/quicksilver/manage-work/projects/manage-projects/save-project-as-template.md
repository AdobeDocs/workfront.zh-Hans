---
product-area: projects;templates
navigation-topic: manage-projects
title: 将项目另存为模板
description: 在项目级别将项目另存为模板另存为模板，以便用户在UI中看到该内容；还有一篇文章提供了更深入的链接（分步）。 此功能需要同时保留在项目和模板区域。)”
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 1%

---

# 将项目另存为模板

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

如果您决定某个项目在未来某个时间再次出现，则可以从现有项目创建模板。 然后，您可以再次使用该模板来创建未来项目，这些项目可能包含类似信息或可能与现有项目共享相同的时间表或工作分配。

## 访问要求

<!--drafted for P&P:
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
   <td> <p>Current license: Standard </p>
   Or 
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you save the project as a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>编辑对模板的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目或更高权限 </p> <p>在将项目另存为模板后，您将获得对模板的管理权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 将项目另存为模板

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

   ![](assets/save-as-template-first-step-350x159.png)

1. 单击&#x200B;**下一步。**
1. 在&#x200B;**选项**&#x200B;部分中，选中要从模板中清除的任何信息旁边的复选框。

   ![](assets/save-as-template-options-step-350x109.png)

1. 单击&#x200B;**下一步。**
1. 在&#x200B;**排除**&#x200B;部分中，选择要从项目中排除的任何任务。

   ![](assets/save-as-template-exclude-350x205.png)

1. 单击&#x200B;**完成并保存模板。**

   您的模板现在显示在可用模板的列表中，并可附加到现有项目或用于创建新项目。
