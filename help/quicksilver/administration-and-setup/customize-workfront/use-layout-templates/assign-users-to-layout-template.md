---
title: 将用户分配给布局模板
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 作为Adobe Workfront管理员，您可以将已创建的布局模板分配给需要使用该布局模板的任何用户、工作角色、团队或组。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# 将用户分配给布局模板

{{preview-fast-release-general}}

您可以将已创建的布局模板分配给需要使用该模板的任何用户、工作角色、团队或组。

对于未分配布局模板的用户，使用默认布局。 要了解默认布局，请参阅[关于默认Adobe Workfront布局](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md)。

用户也可以向自己分配布局模板，如使用布局模板更改我的工作和工作请求区域中所述。

您可以将多个不同的布局模板分配给相同的名称。 有关哪个布局模板对用户、角色、组或团队有效的详细信息，请参阅本文后面的[布局模板分配优先级](#layout-template-assignment-priority)。

有关布局模板的详细信息，请参阅[布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md)。

有关组的布局模板的信息，请参阅[创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问级别。</p>
        <p>要为组执行这些操作，您必须是该组的经理。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将布局模板分配给用户

1. 开始处理布局模板，如[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。

   >[!TIP]
   >
   >当您对布局模板感到满意时，我们建议您对其进行测试，如[测试新布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)中所述。

1. 单击页面顶部的&#x200B;**将此项分配给**。
1. 在出现的框中，单击&#x200B;**添加用户、工作角色、团队或组**，开始键入用户、工作角色、团队或组的名称，然后在此名称出现在下拉列表中时单击它。

   最近添加的名称以蓝色背景显示。 在编辑现有布局模板时，这很有用，因为您可以区分刚刚添加和列表中已存在的名称。

   已分配给其他布局模板的任何用户、工作角色、团队或组的名称右侧将显示一个信息图标![信息图标](assets/info-icon.png)。 您可以将鼠标悬停在图标上以查看该布局模板的名称，并决定是否要覆盖现有分配。

1. 根据需要重复前两个步骤，将布局模板分配给其他用户、工作角色、团队或组。

   一次最多可以分配100个用户。

1. 单击&#x200B;**完成**，然后单击左下角的&#x200B;**保存**&#x200B;或&#x200B;<span class="preview">**保存并关闭**</span>。

   此步骤将完成创建和分配布局模板的过程。

## 布局模板分配优先级 {#layout-template-assignment-priority}

您和其他Workfront管理员可以通过以下四种方式将多个不同的布局模板分配给同一个用户：

* 对个人用户
* 对于用户拥有的特定工作角色
* 对于用户所在的某个团队
* 对于用户所在的某个组

但是，在任意给定时间，用户只能看到一个布局模板。 可见的模板由以下优先级层次结构决定：

* **个人用户**：以个人用户身份分配给该人员的布局模板将覆盖所有其他用户。 您可以通过进行新分配来覆盖以前为单个用户进行的分配；最近的分配优先。
* **主要工作角色**：如果人员未作为单个用户分配布局模板，他们会看到为其主要工作角色分配的模板。

  只有分配给用户的主要工作角色的布局模板对用户可见。 分配给用户所具有的任何辅助工作角色的模板不可见。

* **主团队**：如果人员未作为个人用户或具有主要工作角色的用户分配布局模板，他们将会看到模板分配给其主团队。

  只有分配给用户主团队的模板对用户可见。 分配给用户为成员的其他团队的模板不可见。

* **主组**：如果人员未作为个人用户、具有主要工作角色的用户或主团队成员分配布局模板，他们会看到分配给其主组的模板。

  只有分配给用户“主页”组的模板对用户可见。 分配给其任何其他组的模板不可见。

## 分配给布局模板的大量用户

<!--If you edit a layout template which is assigned to more than 2000 users and make changes to it, only the first 2000 users will be retained on the layout template and will see the changes you made. The layout template is removed from all others.
-->
如果要为布局模板分配超过2000个用户，我们建议您执行以下操作之一：

* 将用户组织到组或团队中，并将布局模板分配给这些组或团队。 有关详细信息，请参阅[创建组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)和[创建和管理团队](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md)。

* 将工作角色分配给用户，并将布局模板分配给其主要工作角色。 有关详细信息，请参阅[创建和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。
