---
product-area: projects;templates
navigation-topic: manage-projects
title: 将项目另存为模板
description: 在项目级别将项目另存为模板另存为模板，以便用户在UI中看到该内容；还有一篇文章提供了更深入的链接（分步）。 此功能需要同时保留在项目和模板区域。)”
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '787'
ht-degree: 1%

---

# 将项目另存为模板

<!--Audited: 6/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

<div class="preview">

此页面上高亮显示的信息是指尚未普遍可用的功能。 它仅在“预览”环境中对所有客户可用。 从预览版本发布的一周后，所有客户还可以在生产环境中使用相同的功能。

有关详细信息，请参阅[接口现代化](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md)。

</div>

如果您决定某个项目在未来某个时间再次出现，则可以从现有项目创建模板。 然后，您可以再次使用该模板来创建未来项目，这些项目可能包含类似信息或可能与现有项目共享相同的时间表或工作分配。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>新增：标准 </p>
   或 
   <p>当前：计划 </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对模板的访问权限</p> /td&gt; 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目或更高权限 </p> <p>在将项目另存为模板后，您将获得对模板的管理权限</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将项目另存为模板

将项目另存为模板在生产环境和预览环境中有所不同。

### 在生产环境中将项目另存为模板

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


<div class="preview">

### 在预览环境中将项目另存为模板

1. 转到要另存为模板的项目。
1. 单击&#x200B;**更多**&#x200B;菜单![更多图标](assets/qs-more-icon-on-an-object.png)，然后单击&#x200B;**另存为模板**。
1. 在&#x200B;**另存为模板**&#x200B;部分中，为模板指定以下信息：

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
     <tr> 
      <td role="rowheader">自定义表单</td> 
      <td>使用下拉列表选择要附加到模板的任何自定义表单。 如果有任何自定义表单已与项目关联，则会显示这些自定义表单中的所有数据字段。<br>在一个模板中最多可以包含10个自定义表单。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击左侧面板中的&#x200B;**自定义Forms**&#x200B;以删除或重新排序表单。

   要重新排列表单，请以正确的顺序拖放表单。
要删除表单，请选择它，然后单击**删除**。 单击&#x200B;**取消**&#x200B;可删除所选的表单。

   另存为模板框中的![自定义表单区域](assets/custom-forms-ara-in-save-as-template-box.png)

1. 如果需要，请更新附加自定义表单中的信息。 信息将传输到模板。

1. 单击左侧面板部分中的&#x200B;**选项**，然后选中要传输到模板的任何信息旁边的复选框。 取消选择的项目不会转移到模板。 默认情况下，将取消选择所有选项。

   另存为模板框中的![选项区域](assets/options-area-in-save-as-template-box.png)

1. 单击左侧面板中的&#x200B;**排除**，然后选择要从项目中排除的任何任务。 默认情况下，将取消选择所有任务。

   ![另存为模板框中的排除区域](assets/exclude-area-save-as-template-box.png)

1. 单击&#x200B;**完成并保存模板。**

   您的模板现在显示在可用模板的列表中，并可附加到现有项目或用于创建新项目。

</span>