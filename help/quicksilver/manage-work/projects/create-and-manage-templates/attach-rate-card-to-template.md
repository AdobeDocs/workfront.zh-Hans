---
content-type: overview
product-area: templates
navigation-topic: financials
title: 将费率卡附加到模板
description: 在将费率卡分配给模板时，费率卡随后将附加到从该模板创建的所有项目。
author: Lisa
feature: Work Management
source-git-commit: 28a1c1cf30c2b4addbcc1b40f5fd65f99685c75c
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 3%

---

# 将费率卡附加到模板

{{highlighted-preview-article-level}}

在将费率卡分配给模板时，费率卡随后将附加到从该模板创建的所有项目。 费率卡会成为项目中的默认费率卡，但如有必要，可以覆盖此费率卡。

有关费率卡的信息，请参阅[管理费率卡](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)。

有关项目模板的信息，请参阅[项目模板概述](/help/quicksilver/manage-work/projects/create-and-manage-templates/project-template-overview.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td>工作流 Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td>标准</td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>编辑对模板的访问权限</td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td>管理对费率卡的权限，并有权编辑记帐费率</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

必须在Workfront中创建要分配给模板的费率卡。 有关详细信息，请参阅[管理费率卡](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)。

必须为布局模板上的模板启用&#x200B;**费率卡**&#x200B;字段。

1. 在布局模板中，单击&#x200B;**自定义用户看到的内容**&#x200B;下的向下箭头，然后单击&#x200B;**模板**。
1. 在&#x200B;**详细信息**&#x200B;部分中，选择&#x200B;**概述**&#x200B;区域中的&#x200B;**费率卡**&#x200B;字段。

   有关详细信息，请参阅[使用布局模板自定义详细信息视图](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

## 将费率卡附加到模板

{{step1-to-templates}}

1. 创建新模板或编辑现有模板。
1. 在“模板详细信息”>“概述”>“模板关联”部分中，在&#x200B;**费率卡**&#x200B;字段中选择费率卡。

   只有您有权使用的费率卡才可供选择。
您可以开始键入费率卡的名称，以缩小结果列表。

   ![选择模板上的费率卡](assets/select-rate-card-on-template.png)

1. 编辑完模板后保存模板。

   有关创建模板的详细信息，请参阅[创建项目模板](/help/quicksilver/manage-work/projects/create-and-manage-templates/create-template.md)。

   有关编辑模板的详细信息，请参阅[编辑项目模板](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md)。

## 将模板应用到项目

1. 使用该模板创建项目。

   可通过多种方式从模板创建项目。 有关信息，请参阅以下文章：

   * [使用模板创建项目](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)
   * [将任务转换为项目](/help/quicksilver/manage-work/tasks/manage-tasks/convert-task-to-project.md)
   * [将问题转化为项目](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md)

   费率卡会自动保存在项目中。 在“新建项目”框的“概述”>“项目关联”部分中，您可以移除费率卡或在&#x200B;**费率卡**&#x200B;字段中选择其他费率卡。

   ![模板中的费率卡显示在项目详细信息中](assets/create-project-from-template-rate-card.png)

   费率卡及其相关费率会显示在项目费率区域中。

   您也可以从项目中移除费率卡，或在费率区域附加其他费率卡。 有关详细信息，请参阅[将费率卡附加到项目](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md)。

   ![对项目](assets/template-rates-on-project.png)上的模板中的卡片进行评分

   >[!NOTE]
   >
   >如果模板上有单个费率，并且费率卡也附加到了模板上，则当您从模板创建项目时，单个费率卡和费率卡都会显示在费率列表中。

1. （可选）要将费率卡应用于现有项目，请将模板附加到项目。

   在模板预览中使用&#x200B;**自定义和附加**&#x200B;选项时，可以在“附加模板”>“选项”部分中选择&#x200B;**费率卡**&#x200B;项，以将费率卡添加到项目中。 清除此复选框，以排除费率卡不转移到项目。

   有关详细信息，请参阅[将模板附加到项目](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md)。

1. （可选）要将费率卡从特定项目保存到模板，请将项目另存为模板。

   在“另存为模板”框的“选项”部分中，您可以选择&#x200B;**费率卡**&#x200B;项以将费率卡添加到模板。 清除复选框，以排除费率卡转移到模板。

   有关详细信息，请参阅[将项目另存为模板](/help/quicksilver/manage-work/projects/manage-projects/save-project-as-template.md)



