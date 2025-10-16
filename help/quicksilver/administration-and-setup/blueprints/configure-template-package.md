---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 配置Blueprint
description: 在安装Blueprint之前，您可以配置项目模板或组织结构的详细信息。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: df10bc8f-b980-4c61-ae6d-bcea03103738
source-git-commit: 5fd855bec596926a4361fd07a1a763c7956e5e61
workflow-type: tm+mt
source-wordcount: '1841'
ht-degree: 0%

---

# 配置Blueprint

您可以在安装Blueprint之前配置其详细信息。 项目模板和组织结构Blueprint类型通常需要设置一些首选项并映射一些属性。 其他Blueprint类型可能不需要配置，您将按原样安装它们。 有关安装的更多信息，请参阅[安装Blueprint](/help/quicksilver/administration-and-setup/blueprints/blueprints-install.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>标准</p>
   <p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>Workfront管理员 </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 配置项目模板Blueprint

1. 查找要使用的Blueprint。
1. 单击&#x200B;**[!UICONTROL 安装]**，然后选择环境：

   <table style="table-layout:auto">
        <tr>
        <td><strong>生产</strong></td>
        <td>生产环境是您的实时环境。</td>
    </tr>
    <tr>
        <td><strong>Sandbox 预览</strong></td>
        <td>沙盒预览是一个测试环境，用作实时环境的副本，每个周末由Workfront刷新。</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1和2</strong></td>
        <td>自定义刷新沙盒是一个单独的测试环境，由您手动刷新。 获取自定义刷新沙盒需要额外付费。</td>
    </tr>
   </table>

1. 请继续阅读以下章节：

   * [[!UICONTROL 模板首选项]](#template-preferences)
   * [[!UICONTROL 角色映射]](#role-mapping)
   * [[!UICONTROL 团队映射]](#team-mapping)
   * [[!UICONTROL 公司映射]g](#company-mapping)
   * [[!UICONTROL 组映射]](#group-mapping)

## [!UICONTROL 模板首选项] {#template-preferences}

选择您希望如何安装模板。

您还可以在安装Blueprint之前指定模板所有权。 安装模板后，您可以更改这些字段。 有关详细信息，请参阅[编辑项目模板](../../manage-work/projects/create-and-manage-templates/edit-templates.md)。

![[!UICONTROL 模板首选项]节](assets/Blueprints_TemplatePreferences.png)

1. 在[!UICONTROL 模板首选项]部分中，指定新的模板名称。
1. 指定以下内容：

   <table style="table-layout:auto">
    <tr>
        <td><strong>[！UICONTROL模板所有者]<strong></td>
        <td>此人将获得模板的[！UICONTROL管理]权限，并在使用模板创建项目时成为项目所有者。</td>
    </tr>
    <tr>
        <td><strong>[！UICONTROL模板发起人]</strong></td>
        <td>此人通常是需要了解项目进展情况的经理、执行人员或利益相关者。 项目发起人不再获得对项目的任何其他访问权限，而是添加到项目的电子邮件通知中。</td>
    </tr>
    <tr>
        <td><strong>[！UICONTROL Portfolio]</strong></td>
        <td>这是项目在创建时将属于的项目组合。</td>
    </tr>
    <tr>
        <td><strong>[！UICONTROL项目]</strong></td>
        <td>这是项目在创建后所属的程序。</td>
    </tr>
   </table>

1. 选择模板是作为活动模板还是非活动模板安装。
1. 如果首选项可用，选择是否要使用定义的新问题首选项。

   单击&#x200B;**[!UICONTROL 查看问题首选项]**&#x200B;以查看将随Blueprint一起安装的特定首选项。 从导入的模板创建的项目对[!UICONTROL 问题]分区中添加的新问题使用这些首选项。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>队列主题组</strong></td> 
      <td> <p>队列主题组为问题或请求定义最高级别的类别。 用户在选择提交请求的位置时，将主题组作为菜单选项查看。 一个主题组可以包含多个队列主题。 有关详细信息，请参阅<a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">创建主题组</a>。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>队列主题</strong></td> 
      <td> <p>队列主题与路由规则结合使用，以分配问题或请求。 它们是用户在输入问题或请求时，在选择主题组后选择的菜单选项。 有关详细信息，请参阅<a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">创建队列主题</a>。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>路由规则</strong></td> 
      <td>路由规则将问题或请求发送给特定工作角色、用户或团队。 他们还可以将请求发送给特定项目，而不是与请求队列关联的项目。 有关详细信息，请参阅<a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">创建路由规则</a>。 </td> 
     </tr> 
    </tbody> 
   </table>

   >[!INFO]
   >
   >**示例：**此Blueprint中的新问题首选项提供了四个队列主题。 用户在创建问题时选择以下主题之一。 （由于只有一个主题组，因此将自动应用该主题组，用户无需选择它。） 当用户完成并提交问题时，传送规则将确定它被分配给哪个工作角色或团队。
   >![新问题偏好设置示例](assets/Blueprints_IssuePrefsDetails.png)
   >![新问题的队列主题](assets/blueprints-newissueqtopicsexample-350x204.png)
   >![问题已路由到工作角色](assets/Blueprints_ProjectShowsIssueAssignment.png)

   >[!TIP]
   >
   >* 使用问题偏好设置有助于在项目中捕获新问题或请求的方式保持一致。
   >* 设置这些首选项不会自动将从模板创建的项目变成请求队列。 有关设置请求队列的信息，请参阅[创建请求队列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。
   >* 并非所有Blueprint都包含新的问题首选项。


## [!UICONTROL 角色映射] {#role-mapping}

>[!NOTE]
>
>此部分可能不会出现在某些Blueprint中。

某些模板包含规定的工作角色。 当模板转化为项目时，工作角色可帮助您分配合适的人员。 在安装Blueprint之前，您可以自定义角色的映射方式。 单击&#x200B;**[!UICONTROL 查看角色描述]**&#x200B;以了解有关Blueprint中可用角色的更多信息。

Blueprint按角色名称进行搜索，以查看是否有任何现有角色匹配。 搜索区分大小写，因此名称必须完全匹配。 如果没有匹配的现有角色，您可以让Blueprint为您创建它们。

![[!UICONTROL 角色映射]节](assets/Blueprints_RoleMapping.png)

1. 如果角色存在，您可以选择以下选项之一：

   1. 使用其他名称创建新角色，然后在文本框中键入该名称。
   1. 使用现有角色，然后在选择框中选择角色。
   1. 不要使用映射的角色。 不建议使用此选项，因为某些任务将不会分配角色。

1. 如果角色不存在，您可以选择以下选项之一：

   1. 创建新角色。 此选项将创建Blueprint推荐的角色。
   1. 使用其他名称创建新角色，然后在文本框中键入该名称。
   1. 使用现有角色，然后在选择框中选择角色。
   1. 不要使用映射的角色。 不建议使用此选项，因为某些任务将不会分配角色。

>[!NOTE]
>
>安装过程不会将角色应用于特定人员。 安装Blueprint解决方案后，您应该验证这些角色中的人员，并根据需要分配人员。 有关信息，请参阅安装Blueprint后要执行的[操作](../../administration-and-setup/blueprints/best-next-actions-after-install.md)。

有关[!DNL Workfront]中工作角色的更多信息，请参阅[创建和管理工作角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

## [!UICONTROL 团队映射] {#team-mapping}

>[!NOTE]
>
>此部分可能不会出现在某些Blueprint中。

某些模板包含规定的团队。 团队的任何成员都可以完成分配给团队的工作。 在安装Blueprint之前，您可以自定义团队的映射方式。 单击&#x200B;**[!UICONTROL 查看团队描述]**&#x200B;以了解有关Blueprint中可用团队的更多信息。

Blueprint按团队名称搜索，以查看是否有任何现有团队匹配。 搜索区分大小写，因此名称必须完全匹配。 如果没有匹配的现有团队，您可以让Blueprint为您创建它们。

![[!UICONTROL 团队映射]节](assets/Blueprints_TeamMapping.png)

1. 如果存在团队，您可以选择以下选项之一：

   1. 使用其他名称创建新团队，然后在文本框中键入名称。
   1. 使用[!UICONTROL 现有团队]，然后在选择框中选择一个团队。
   1. 不使用映射的团队。 不建议使用此选项，因为某些任务将不会分配团队。

1. 如果团队不存在，您可以选择以下选项之一：

   1. 创建新团队。 此选项将创建Blueprint推荐的团队。
   1. 使用其他名称创建新团队，然后在文本框中键入名称。
   1. 使用[!UICONTROL 现有团队]，然后在选择框中选择一个团队。
   1. 不使用映射的团队。 不建议使用此选项，因为某些任务将不会分配团队。

>[!NOTE]
>
>安装过程不会将人员添加到团队。 您应在安装Blueprint解决方案后验证团队中的人员，并在必要时分配人员。 有关信息，请参阅安装Blueprint后要执行的[操作](../../administration-and-setup/blueprints/best-next-actions-after-install.md)。

有关团队如何在[!DNL Workfront]中工作的更多信息，请参阅[创建和管理团队](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md)。

## 公司映射 {#company-mapping}

>[!NOTE]
>
>此部分可能不会出现在某些Blueprint中。

一些蓝图包括规定的公司。 公司是一个组织单位，可以代表您的组织、组织内的部门或与您合作的客户。 在安装Blueprint之前，您可以自定义公司的映射方式。 单击&#x200B;**[!UICONTROL 查看公司描述]**&#x200B;以详细了解Blueprint中可用的公司。

Blueprint按公司名称搜索，以查看是否有任何现有公司匹配。 搜索区分大小写，因此名称必须完全匹配。 如果没有匹配的现有公司，您可以让Blueprint为您创建它们。 Blueprint中的主要公司映射到您环境中的主要公司，即使它们没有相同的名称。

![[!UICONTROL 公司映射]节](assets/Blueprints_CompanyMapping.png)

1. 如果公司存在，您可以选择以下选项之一：

   1. 使用其他名称创建新公司，然后在文本框中键入该名称。
   1. 使用现有公司，然后在选择框中选择公司。\

      Blueprint中的主要公司映射到您环境中的主要公司，即使它们没有相同的名称。
   1. 不要使用映射的公司。 不建议使用此选项，因为其他对象中的公司引用将为空。

1. 如果公司不存在，您可以选择以下选项之一：

   1. 创建新公司。 此选项将创建Blueprint推荐的公司。
   1. 使用其他名称创建新公司，然后在文本框中键入该名称。
   1. 使用现有公司，然后在选择框中选择公司。
   1. 不要使用映射的公司。 不建议使用此选项，因为其他对象中的公司引用将为空。

>[!NOTE]
>
>要在安装Blueprint后配置公司，请参阅安装Blueprint后要执行的[操作](../../administration-and-setup/blueprints/best-next-actions-after-install.md)。

有关将模板与公司关联的信息，请参阅[编辑项目模板](../../manage-work/projects/create-and-manage-templates/edit-templates.md)。

有关公司如何在[!DNL Workfront]中运行的信息，请参阅[创建和编辑公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

## [!UICONTROL 组映射] {#group-mapping}

>[!NOTE]
>
>此部分可能不会出现在某些Blueprint中。

一些Blueprint包含规定组。 组是一组用户，与您的部门结构一致。 组与Workfront中的团队和公司类似，但与之不同。 在安装Blueprint之前，您可以自定义组的映射方式。 单击&#x200B;**[!UICONTROL 查看组描述]**&#x200B;以了解有关Blueprint中可用组的更多信息。

Blueprint按组名搜索，以查看是否有任何现有组匹配。 搜索区分大小写，因此名称必须完全匹配。 如果没有匹配的现有组，您可以让Blueprint为您创建它们。

![[!UICONTROL 组映射]节](assets/Blueprints_GroupMapping.png)

1. 如果存在组，则可以选择&#x200B;**[!UICONTROL 重新映射组]**&#x200B;并选择以下选项之一：

   1. **[!UICONTROL 使用其他名称创建新组]**，然后键入要分配给此组的名称。 对Blueprint定义中组的引用将改为关联到此新组。
   1. **[!UICONTROL 替换为现有组]**，然后在选择框中搜索并选择组。

      >[!NOTE]
      >
      >不能重命名现有组。

1. 如果组不存在，您可以：

   1. 在文本框中键入建议的组名以更改该组名。
   1. 选择&#x200B;**[!UICONTROL 重新映射组]**&#x200B;并选择[!UICONTROL 替换为现有组]，然后在选择框中搜索并选择组。
   1. 选择&#x200B;**[!UICONTROL 重新映射组]**&#x200B;并选择&#x200B;**[!UICONTROL 插入现有组]**，然后在选择框中搜索并选择组。 此选项将在现有组下创建新子组。

>[!NOTE]
>
>要在安装Blueprint后配置组，请参阅安装Blueprint后要执行的[操作](../../administration-and-setup/blueprints/best-next-actions-after-install.md)。

有关在[!DNL Workfront]中使用群组的信息，请参阅[群组概述](../../administration-and-setup/manage-groups/groups-overview/groups.md)。
