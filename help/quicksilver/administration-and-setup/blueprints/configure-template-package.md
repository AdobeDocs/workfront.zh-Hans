---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 配置Blueprint
description: 在安装Blueprint之前，您可以配置项目模板或组织结构的详细信息。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: df10bc8f-b980-4c61-ae6d-bcea03103738
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1824'
ht-degree: 0%

---

# 配置Blueprint

您可以在安装Blueprint之前配置其详细信息。 项目模板和组织结构蓝图类型通常要求设置一些首选项并映射某些属性。 其他Blueprint类型可能不需要配置，您将按原样安装它们。 有关安装的详细信息，请参阅 [安装Blueprint](/help/quicksilver/administration-and-setup/blueprints/blueprints-install.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划</strong></td>
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 许可证</strong></td>
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td>
   <td> <p>[!UICONTROL系统管理员]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 配置项目模板Blueprint

1. 查找要使用的蓝图。
1. 单击 **[!UICONTROL 安装]**，然后选择环境：

   <table style="table-layout:auto">
        <tr>
        <td><strong>生产</strong></td>
        <td>生产是您的实时环境。</td>
    </tr>
    <tr>
        <td><strong>Sandbox 预览</strong></td>
        <td>“沙盒预览”是一个测试环境，可用作实时环境的副本，并且每周末由Workfront刷新一次。</td>
    </tr>
    <tr>
        <td><strong>沙盒1和2</strong></td>
        <td>自定义刷新沙盒是一个单独的测试环境，由您手动刷新。 获取“自定义刷新”沙盒需要额外付费。</td>
    </tr>
   </table>

1. 继续以下部分：

   * [[!UICONTROL 模板首选项]](#template-preferences)
   * [[!UICONTROL 角色映射]](#role-mapping)
   * [[!UICONTROL 团队映射]](#team-mapping)
   * [[!UICONTROL 公司映射]g](#company-mapping)
   * [[!UICONTROL 组映射]](#group-mapping)

## [!UICONTROL 模板首选项] {#template-preferences}

选择安装模板的方式。

在安装Blueprint之前，您还可以指定模板所有权。 安装模板后，您可以对这些字段进行更改。 有关更多信息，请参阅 [编辑项目模板](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

![[!UICONTROL 模板首选项] 部分](assets/Blueprints_TemplatePreferences.png)

1. 在 [!UICONTROL 模板首选项] 部分，指定新的模板名称。
1. 指定以下内容：

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL模板所有者]<strong></td>
        <td>此人员将收到对模板的[!UICONTROL管理]权限，并在使用模板创建项目时成为项目所有者。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL模板发起者]</strong></td>
        <td>此人通常是经理、高管或利益相关方，需要了解项目的进展情况。 项目赞助商不会获得对项目的任何其他访问权限，但会添加到项目的电子邮件通知中。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROLPortfolio]</strong></td>
        <td>这是项目创建时所属的项目组合。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Program]</strong></td>
        <td>这是项目创建时所属的项目。</td>
    </tr>
   </table>

1. 选择模板是安装为活动模板还是非活动模板。
1. 如果首选项可用，请选择是否要使用定义的新问题首选项。

   单击 **[!UICONTROL 请参阅问题首选项]** 查看将与blueprint一起安装的特定首选项。 使用导入的模板创建的项目会使用这些首选项来解决在 [!UICONTROL 问题] 中。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>队列主题组</strong></td> 
      <td> <p>队列主题组为问题或请求定义最高级别的类别。 用户在选择提交请求的位置时，会将主题组视为菜单选项。 一个主题组可以包含多个队列主题。 有关更多信息，请参阅 <a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">创建主题组</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>队列主题</strong></td> 
      <td> <p>队列主题与路由规则结合使用来分配问题或请求。 这些是用户在选择主题组后输入问题或请求时选择的菜单选项。 有关更多信息，请参阅 <a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">创建队列主题</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>路由规则</strong></td> 
      <td>路由规则将问题或请求发送给特定作业角色、用户或团队。 他们还可以将请求发送到特定项目，而不是与请求队列关联的项目。 有关更多信息，请参阅 <a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">创建路由规则</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!INFO]
   >
   >**示例：** 此Blueprint中的新问题首选项提供了四个队列主题。 用户在创建问题时会选择以下主题之一。 （由于只存在一个主题组，因此会自动应用该主题组，用户无需选择该主题组。） 当用户完成并提交问题时，路由规则将确定分配给哪个作业角色或团队。
   >![新问题首选项示例](assets/Blueprints_IssuePrefsDetails.png)
   >![新问题的队列主题](assets/blueprints-newissueqtopicsexample-350x204.png)
   >![已路由到工作角色的问题](assets/Blueprints_ProjectShowsIssueAssignment.png)

   >[!TIP]
   >
   >* 使用问题首选项有助于创建在项目中捕获新问题或请求的一致性。
   >* 设置这些首选项不会自动将从模板创建的项目放入请求队列。 有关设置请求队列的信息，请参阅 [创建请求队列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   >* 并非所有蓝图都包含新的问题首选项。



## [!UICONTROL 角色映射] {#role-mapping}

>[!NOTE]
>
>某些蓝图中可能没有此部分。

某些模板包括规定的工作角色。 作业角色可帮助您在模板转换为项目时分配适当的人员。 在安装Blueprint之前，您可以自定义角色的映射方式。 单击 **[!UICONTROL 请参阅角色描述]** 了解有关blueprint中可用角色的更多信息。

Blueprint会按角色名称搜索，以查看现有角色是否匹配。 搜索区分大小写，因此名称必须完全匹配。 如果现有角色不匹配，您可以让Blueprint为您创建它们。

![[!UICONTROL 角色映射] 部分](assets/Blueprints_RoleMapping.png)

1. 如果存在角色，您可以选择以下选项之一：

   1. 使用其他名称创建新角色，然后在文本框中键入该名称。
   1. 使用现有角色，然后在选择框中选择角色。
   1. 请勿使用映射的角色。 不建议使用此选项，因为某些任务不会分配角色。

1. 如果角色不存在，您可以选择以下选项之一：

   1. 创建新角色。 此选项将创建Blueprint推荐的角色。
   1. 使用其他名称创建新角色，然后在文本框中键入该名称。
   1. 使用现有角色，然后在选择框中选择角色。
   1. 请勿使用映射的角色。 不建议使用此选项，因为某些任务不会分配角色。

>[!NOTE]
>
>安装过程不会将角色应用到特定人员。 您应在安装Blueprint解决方案后验证这些角色中的人员，并在必要时分配人员。 有关信息，请参阅 [安装Blueprint后要执行的操作](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

有关 [!DNL Workfront]，请参阅 [创建和管理作业角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## [!UICONTROL 团队映射] {#team-mapping}

>[!NOTE]
>
>某些蓝图中可能没有此部分。

有些模板包括规定的团队。 分配给团队的工作可由团队的任何成员完成。 在安装Blueprint之前，您可以自定义如何映射团队。 单击 **[!UICONTROL 请参阅团队描述]** 了解有关blueprint中可用团队的更多信息。

Blueprint会按团队名称搜索，以查看现有团队是否匹配。 搜索区分大小写，因此名称必须完全匹配。 如果现有团队不匹配，您可以让Blueprint为您创建它们。

![[!UICONTROL 团队映射] 部分](assets/Blueprints_TeamMapping.png)

1. 如果存在团队，您可以选择以下选项之一：

   1. 使用其他名称创建新团队，然后在文本框中键入该名称。
   1. 使用 [!UICONTROL 现有团队]，然后在选择框中选择团队。
   1. 请勿使用映射的团队。 不建议使用此选项，因为某些任务不会分配团队。

1. 如果团队不存在，您可以选择以下选项之一：

   1. 创建新团队。 此选项会创建Blueprint推荐的团队。
   1. 使用其他名称创建新团队，然后在文本框中键入该名称。
   1. 使用 [!UICONTROL 现有团队]，然后在选择框中选择团队。
   1. 请勿使用映射的团队。 不建议使用此选项，因为某些任务不会分配团队。

>[!NOTE]
>
>安装过程不会向团队添加人员。 您应在安装Blueprint解决方案后验证团队中的人员，并在必要时分配人员。 有关信息，请参阅 [安装Blueprint后要执行的操作](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

有关团队在 [!DNL Workfront]，请参阅 [创建和管理团队](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

## 公司映射 {#company-mapping}

>[!NOTE]
>
>某些蓝图中可能没有此部分。

一些蓝图包括指定公司。 公司是一个组织单位，可以代表您的组织、组织内的部门，或您与之合作的客户。 在安装Blueprint之前，您可以自定义公司的映射方式。 单击 **[!UICONTROL 请参阅公司描述]** 以详细了解Blueprint中提供的公司。

Blueprint会按公司名称搜索，以查看是否存在任何现有公司匹配。 搜索区分大小写，因此名称必须完全匹配。 如果现有公司不匹配，您可以让Blueprint为您创建它们。 Blueprint中的主公司会映射到您环境中的主公司，即使它们没有相同的名称也是如此。

![[!UICONTROL 公司映射] 部分](assets/Blueprints_CompanyMapping.png)

1. 如果公司存在，您可以选择以下选项之一：

   1. 使用其他名称创建新公司，然后在文本框中键入该名称。
   1. 使用现有公司，然后在选择框中选择公司。\

      Blueprint中的主公司会映射到您环境中的主公司，即使它们没有相同的名称也是如此。
   1. 请勿使用映射的公司。 不建议使用此选项，因为公司在其他对象中的引用将为空。

1. 如果公司不存在，您可以选择以下选项之一：

   1. 创建新的公司. 此选项将创建Blueprint推荐的公司。
   1. 使用其他名称创建新公司，然后在文本框中键入该名称。
   1. 使用现有公司，然后在选择框中选择公司。
   1. 请勿使用映射的公司。 不建议使用此选项，因为公司在其他对象中的引用将为空。

>[!NOTE]
>
>要在安装Blueprint后配置公司，请参阅 [安装Blueprint后要执行的操作](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

有关将模板与公司关联的信息，请参阅 [编辑项目模板](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

有关公司在 [!DNL Workfront]，请参阅 [创建和编辑公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## [!UICONTROL 组映射] {#group-mapping}

>[!NOTE]
>
>某些蓝图中可能没有此部分。

有些蓝图包括预定的组。 组是与部门结构一致的一组用户。 组与Workfront的团队和公司相似，但不同。 在安装Blueprint之前，您可以自定义组的映射方式。 单击 **[!UICONTROL 请参阅群组描述]** 了解有关Blueprint中可用组的更多信息。

Blueprint会按组名称搜索，以查看是否存在任何现有组匹配。 搜索区分大小写，因此名称必须完全匹配。 如果没有与现有组匹配的组，您可以让Blueprint为您创建它们。

![[!UICONTROL 组映射] 部分](assets/Blueprints_GroupMapping.png)

1. 如果存在群组，则可以选择 **[!UICONTROL 重新映射组]** 并选择以下选项之一：

   1. **[!UICONTROL 使用其他名称创建新组]**，然后键入要分配给此群组的名称。 在Blueprint定义中对组的引用将与此新组关联。
   1. **[!UICONTROL 替换为现有组]**，然后在选择框中搜索并选择群组。

      >[!NOTE]
      >
      >无法重命名现有组。

1. 如果组不存在，您可以：

   1. 在文本框中键入相应的组名称，以更改建议的组名称。
   1. 选择 **[!UICONTROL 重新映射组]** 选择 [!UICONTROL 替换为现有组]，然后在选择框中搜索并选择群组。
   1. 选择 **[!UICONTROL 重新映射组]** 选择 **[!UICONTROL 在现有组下插入]**，然后在选择框中搜索并选择群组。 此选项在现有组下创建新子组。

>[!NOTE]
>
>要在安装Blueprint后配置组，请参阅 [安装Blueprint后要执行的操作](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

有关在中使用组的信息 [!DNL Workfront]，请参阅 [群组概述](../../administration-and-setup/manage-groups/groups-overview/groups.md).
