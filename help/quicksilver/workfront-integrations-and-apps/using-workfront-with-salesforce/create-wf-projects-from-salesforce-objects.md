---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: 创建 [!DNL Adobe Workfront] 项目 [!DNL Salesforce] 对象
description: 安装后 [!DNL Adobe Workfront] 对于Salesforce，您可以定义创建 [!DNL Workfront] 符合特定条件的项目 [!DNL Salesforce] 机会和帐户。
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '1506'
ht-degree: 3%

---

# 创建 [!DNL Adobe Workfront] 项目 [!DNL Salesforce] 对象

安装后 [!DNL Adobe Workfront] 对于Salesforce，您可以定义创建 [!DNL Workfront] 符合特定条件的项目 [!DNL Salesforce] [!UICONTROL 机会] 和 [!UICONTROL 帐户].

## 访问要求

您必须具有以下访问权限才能使用本文中描述的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL计划]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 先决条件

提交 [!DNL Workfront] 来自 [!DNL Salesforce] [!UICONTROL 机会] 或者，请确保您的环境中具有以下功能：

* 您的 [!DNL Workfront] 管理员已安装 [!DNL Workfront for Salesforce].\
   有关安装的详细信息 [!DNL Workfront for Salesforce]，请参阅 [安装 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* 您的 [!DNL Workfront] 管理员已添加 [!DNL Workfront] 的 [!UICONTROL 机会] 和帐户页面布局。\
   有关添加 [!DNL Workfront] 到页面布局的部分，请参阅 [配置 [!DNL Adobe Workfront] 部分 [!DNL Salesforce] 用户](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* 您拥有 [!DNL Workfront] 帐户，您可以从登录到该帐户 [!DNL Workfront] 部分 [!UICONTROL 机会] 或帐户。

## 配置创建 [!DNL Workfront] 项目来源 [!DNL Salesforce]

* [了解项目的自动创建](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [配置触发器](#configuring-triggers-configuring-triggers)
* [了解项目名称](#understanding-project-names-understanding-project-names)

### 了解项目的自动创建 {#understanding-the-automatic-creation-of-projects}

作为 [!DNL Salesforce] 系统管理员，您可以定义触发器，以在 [!DNL Workfront] 在 [!DNL Salesforce]:

* 的 [!UICONTROL 阶段] a [!UICONTROL 机会] 更新。
* 的 [!UICONTROL 类型] 帐户的名称。

只有在安装了触发器后，才能配置触发器 [!DNL Workfront for Salesforce].  \
有关安装的信息 [!DNL Workfront for Salesforce]，请参阅 [安装 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

在将触发器配置为自动创建时，请考虑以下事项 [!DNL Workfront] 项目 [!DNL Salesforce] 创建或更新项目：

* 你必须是 [!DNL Salesforce] 和 [!DNL Workfront] 系统管理员来配置触发器。
* 配置触发器后，任何更新 [!UICONTROL 阶段] a [!UICONTROL 机会] 或 [!UICONTROL 类型] 帐户可触发创建 [!DNL Workfront] 项目。 这包括 [!DNL Salesforce] 没有 [!DNL Workfront] 帐户。
* 您可以拥有的触发器数量没有限制。
* 您不能基于相同的条件创建多个触发器。 默认情况下，触发器是唯一的。
* 项目创建后，会自动将其链接到该业务机会或生成该项目的帐户。 建立后，此链接将无法断开。
* 一个机会或帐户可以关联到 [!DNL Workfront] 在机会或帐户的生命周期中多次满足触发条件时。

   例如，如果您定义多个 [!UICONTROL 阶段] 对于 [!UICONTROL 机会] 要触发项目，将为机会到达的每个定义阶段创建一个项目，以在该机会的生命周期内触发该项目。 此外，如果您更新 [!UICONTROL 阶段] a [!UICONTROL 机会] 从一个定义的阶段更新到另一个阶段，然后将其更新回定义的阶段，在您第二次更新时将创建第二个项目 [!UICONTROL 阶段] 字段。

* 中的一个项目 [!DNL Workfront] 只能关联到中的一个机会或一个帐户 [!DNL Salesforce] 在任何指定时间，但不能同时对两者。

### 配置触发器 {#configuring-triggers}

配置触发器后，创建 [!DNL Workfront] 为这两个 [!UICONTROL Salesforce Classic] 或 [!DNL Lightning Experience] 框架。

在中配置触发器 [!UICONTROL Salesforce]:

1. 登录到 [!DNL Salesforce] 作为系统管理员。
1. （视情况而定）输入 [!DNL Salesforce Classic]，单击 **[!UICONTROL 设置]**，下 **[!UICONTROL 生成]** 部分，展开 **[!UICONTROL 闪电]**.

   或

   在 [!DNL Salesforce] Lightning Experience，单击 **[!UICONTROL 设置] 图标**，则 **[!UICONTROL 设置]**，在 **[!UICONTROL 平台工具]** 展开 **[!UICONTROL 应用程序]**.

1. 单击 **[!UICONTROL 已安装的包]**.

   请注意， **[!DNL Workfront]** 包已安装。

1. 单击 **[!UICONTROL 配置]** 下一页 **[!DNL Workfront]**.

1. 登录到 [!DNL Workfront] 作为系统管理员。

   的 **[!UICONTROL 触发器]** 页面。

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. 单击 **[!UICONTROL 新触发器]**.
1. 从 **[!UICONTROL [!DNL Salesforce]对象]** 下拉菜单，选择 **[!UICONTROL 机会]**.

   这是必填字段。

1. （视情况而定）指定以下内容：

   1. 从 **[!UICONTROL 阶段]** 下拉菜单中，选择 **[!UICONTROL 阶段]**.\

      当机会到达 [!UICONTROL 阶段] 在此指定，将在中创建项目 [!DNL Workfront]. 这是必填字段。

   1. 在 **[!UICONTROL Portfolio或项目]** 字段中，开始键入要将项目放置到其中的Portfolio或项目群的名称 [!DNL Workfront]，然后在列表中显示时选择它。\

      如果您没有指定Portfolio或项目群，则会创建新项目并将其添加到 [!UICONTROL 我拥有的项目] 登录用户列表 [!DNL Workfront] 配置触发器时。 该用户也是新项目的项目所有者。

   1. 开始键入要与新模板关联的模板名称 [!DNL Workfront] 项目，然后在列表中显示该项目时将其选中。\

      这是必填字段。


      >[!NOTE]
      >
      >如果您在计划用于此集成的模板上指定了模板所有者，则该模板将成为新项目的项目所有者。 新项目显示在 [!UICONTROL 我拥有的项目] 根据模板，新项目所有者的用户列表。

   1. （可选）选择 **[!UICONTROL 为每个已销售的产品类型创建新项目] 字段**，如果您要为在任何一次机会下销售的每种产品类型创建新项目。
   1. （视情况而定）选择 **[!UICONTROL 产品]** 在 **[!UICONTROL 产品]** 下拉菜单。

      这是必填字段。

   1. （视情况而定）开始键入 **[!UICONTROL 模板]** 你想和新 [!DNL Workfront] 项目(如果指定的产品在 [!UICONTROL 机会]. 当列表中显示时选择它。

      这是必填字段。

      将新产品添加到 [!DNL Salesforce] 机会位于为该机会选择的同一Portfolio或项目中。

      >[!IMPORTANT]
      >
      >仅在 [!UICONTROL 机会]. 为更新“暂存”字段时指定的每个产品创建一个唯一的项目，而不是在产品被添加到 [!UICONTROL 机会].

1. （可选）单击 **[!UICONTROL 新触发器]**.
1. （可选）从 **[!UICONTROL [!DNL Salesforce]对象]** 下拉菜单中，选择**帐户**。

   这是必填字段。
1. （视情况而定）指定以下内容：

   1. 选择 **[!UICONTROL 类型]** 从 **[!UICONTROL 类型]** 下拉菜单。

      当任何**户**被指定为 **[!UICONTROL 类型]** 此处指定 [!DNL Salesforce], a **[!UICONTROL 项目]** 创建于 [!DNL Workfront].

      这是必填字段。

   1. （可选）开始键入 **[!UICONTROL Portfolio]** 或 **[!UICONTROL 项目]** 希望将项目放入的位置 [!DNL Workfront] 在 **[!UICONTROL Portfolio或项目]** 字段，然后在列表中显示时将其选中。

      如果您没有指定Portfolio或项目群，则会创建新项目并将其添加到 **[!UICONTROL 我拥有的项目]** 登录用户列表 [!DNL Workfront] 从 [!DNL Salesforce]. 用户也是新项目的项目所有者。

   1. 开始键入 **[!UICONTROL 模板]** 你想和新 [!DNL Workfront] 项目，然后在列表中显示该项目时将其选中。

      这是必填字段。

      >[!NOTE]
      >
      >如果您在计划用于此集成的模板上指定了模板所有者，则该模板将成为新项目的项目所有者。 新项目显示在 **[!UICONTROL 我拥有的项目]** 根据模板，新项目所有者的用户列表。
   ![salesforce_triggers_page_with_cleaned_up_template_names_png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. 单击&#x200B;**[!UICONTROL 保存]**。

   [!DNL Workfront] 现在，每当满足任何触发器时，都会生成项目。

### 了解项目名称 {#understanding-project-names}

根据生成项目的触发器，中项目的名称 [!DNL Workfront] 可以遵循以下任一模式：

* 如果项目是基于业务机会或帐户触发器创建的，则项目的名称为： *`<Salesforce object name>`: `<Project template name>` (通过 [!DNL Salesforce])*.
* 如果项目是基于一个机会触发器创建的，该触发器还包含添加新产品，则项目的名称为： *`<Salesforce object name>`: `<Salesforce product name>` (通过 [!DNL Salesforce])*.

## 查看 [!DNL Workfront] 项目

如果 [!DNL Workfront] 管理员已添加 [!DNL Workfront] 的 [!UICONTROL 机会] 或帐户页面布局，您可以在 [!UICONTROL 项目] 选项卡。\
有关添加 [!DNL Workfront] 的页面布局 [!UICONTROL 机会] 或帐户，请参阅 [配置 [!DNL Adobe Workfront] 部分 [!DNL Salesforce] 用户](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

您必须具有 [!DNL Workfront] 帐户并登录到 [!DNL Workfront] 查看 [!UICONTROL 项目] 选项卡。

查看从 [!UICONTROL 机会] 或帐户：

1. 转到 [!UICONTROL 机会] 或帐户。
1. 转到 **[!DNL Workfront]** 中。

   >[!NOTE]
   >
   >根据 [!DNL Workfront] 管理员配置了此部分，可能具有不同的名称。

1. 选择 **[!UICONTROL 项目]** 选项卡。

   由定义的触发器创建的所有项目都将在此选项卡中列出。 中的任何用户 [!DNL Salesforce] 也有 [!DNL Workfront] 帐户以及有权在 [!DNL Workfront] 也可以在 [!DNL Salesforce] 对于 [!UICONTROL 机会] 或生成这些帐户的帐户。

   您可以查看有关该集成所创建项目的以下信息：

   * 项目名称
   * 参考号
   * 输入日期
   * 所有者的名称
   * 状态
   * 完成情况
   * 计划完成日期
   * 完成百分比

      此信息在 [!DNL Workfront]，则可以查看此列表中更新的字段。

1. （可选）单击项目的名称以在Workfront中将其打开。
1. （可选）单击 [!UICONTROL **[!UICONTROL 转到Salesforce]**] 在 [!UICONTROL 项目详细信息] 访问 [!UICONTROL 机会] 或项目源的帐户。 您的系统或组管理员必须将 [!UICONTROL 集成] 字段，以在项目标题中查找。

   >[!NOTE]
   >
   >的 [!UICONTROL 转到Salesforce] 链接对所有 [!DNL Workfront] 可以查看项目的用户。 您必须具有 [!DNL Salesforce] 帐户 [!DNL Salesforce] 从中生成项目的机会或帐户。
