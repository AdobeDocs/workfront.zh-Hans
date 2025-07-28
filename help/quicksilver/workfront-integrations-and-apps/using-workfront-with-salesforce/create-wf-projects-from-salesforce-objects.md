---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: 从 [!DNL Adobe Workfront] 对象创建 [!DNL Salesforce] 项目
description: 安装Salesforce的 [!DNL Adobe Workfront] 后，您可以定义在满足 [!DNL Workfront] 机会和帐户的特定条件时创建 [!DNL Salesforce] 项目的触发器。
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '1581'
ht-degree: 3%

---

# 从[!DNL Adobe Workfront]对象创建[!DNL Salesforce]项目

>[!IMPORTANT]
>
>为了提供更稳定和可扩展的集成，我们正在使用Workfront自动化与集成(Fusion)转向一种现代、灵活的集成方法。 在此过渡过程中，Workfront for Salesforce集成在&#x200B;**2026年2月28日**&#x200B;后不可用。
>
>为了满足贵组织与Salesforce的集成需求，我们建议使用Workfront自动化和集成。
>
>有关Workfront自动化和集成的概述，请参阅[Adobe Workfront Fusion概述](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>有关Salesforce的Workfront自动化和集成模块的特定功能的信息，请参阅[Salesforce模块](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules)。

为Salesforce安装[!DNL Adobe Workfront]后，您可以定义在[!DNL Workfront] [!DNL Salesforce]机会[!UICONTROL 和]帐户[!UICONTROL 上满足某些条件时创建]项目的触发器。

## 访问要求

您必须具有以下权限才能使用本文中所述的功能：

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
   <td> <p>[!UICONTROL 计划]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 先决条件

从[!DNL Workfront] [!DNL Salesforce]机会[!UICONTROL 或帐户提交]请求
确保您的环境中具有以下内容：

* 您的[!DNL Workfront]管理员已安装[!DNL Workfront for Salesforce]。\
   有关安装[!DNL Workfront for Salesforce]的详细信息，请参阅[安装 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* 您的[!DNL Workfront]管理员已将[!DNL Workfront]部分添加到您的[!UICONTROL 机会]和帐户
页面布局。\
   有关将[!DNL Workfront]分区添加到页面布局的详细信息，请参阅[为 [!DNL Adobe Workfront] 用户配置 [!DNL Salesforce] 分区](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)。

* 您拥有[!DNL Workfront]帐户，可以从[!DNL Workfront]Opportunity[!UICONTROL 或帐户中的]部分登录到该帐户
.

## 配置从[!DNL Workfront]创建[!DNL Salesforce]个项目

* [了解项目的自动创建](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [配置触发器](#configuring-triggers-configuring-triggers)
* [了解项目名称](#understanding-project-names-understanding-project-names)

### 了解项目的自动创建 {#understanding-the-automatic-creation-of-projects}

作为[!DNL Salesforce]系统管理员，您可以定义在[!DNL Workfront]中发生以下情况时可在[!DNL Salesforce]中自动创建项目的触发器：

* [!UICONTROL Opportunity]的[!UICONTROL 阶段]已更新。
* 帐户的[!UICONTROL 类型]
已更新。

只有在安装了[!DNL Workfront for Salesforce]之后，才能配置触发器。  \
有关安装[!DNL Workfront for Salesforce]的信息，请参阅[安装 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)。

在创建或更新[!DNL Workfront]项时配置触发器以自动创建[!DNL Salesforce]项目时，请考虑以下事项：

* 您必须是[!DNL Salesforce]和[!DNL Workfront]系统管理员才能配置触发器。
* 配置触发器后，任何更新[!UICONTROL Opportunity]的[!UICONTROL 阶段]或帐户的[!UICONTROL 类型]的人
可以触发创建[!DNL Workfront]项目。 这包括没有[!DNL Salesforce]帐户的[!DNL Workfront]用户。
* 您可以触发的触发器数量没有限制。
* 您不能根据相同条件创建多个触发器。 默认情况下，触发器是唯一的。
* 项目创建后，将自动链接到商机或生成它的帐户。 建立后，此链接将无法断开。
* 当在机会或帐户的生命周期中多次满足触发的条件时，一个机会或帐户可以链接到[!DNL Workfront]中的多个项目。

  例如，如果您为[!UICONTROL 机会]定义多个[!UICONTROL 阶段]以触发项目，则会在机会生命周期内为机会达到的每个已定义阶段创建一个项目。 此外，如果您将[!UICONTROL Opportunity]的[!UICONTROL 阶段]从一个已定义的阶段更新到另一个已定义的阶段，然后将其更新回已定义的阶段，则会在您第二次将[!UICONTROL 阶段]字段更新到同一已定义的阶段时创建另一个项目。

* [!DNL Workfront]中的一个项目在任何给定时间只能链接到[!DNL Salesforce]中的一个机会或一个帐户，但不能同时链接到两者。

### 配置触发器 {#configuring-triggers}

配置触发器后，将为[!DNL Workfront]Salesforce Classic[!UICONTROL 或]框架启用创建[!DNL Lightning Experience]项目的过程。

要在[!UICONTROL Salesforce]中配置触发器，请执行以下操作：

1. 以系统管理员身份登录到[!DNL Salesforce]。
1. （视情况而定）在[!DNL Salesforce Classic]中，单击&#x200B;**[!UICONTROL 设置]**，然后在&#x200B;**[!UICONTROL 生成]**&#x200B;部分下，展开&#x200B;**[!UICONTROL 闪电]**。

   或

   在[!DNL Salesforce] Lightning Experience中，单击&#x200B;**[!UICONTROL 设置]图标**，然后单击&#x200B;**[!UICONTROL 设置]**，在&#x200B;**[!UICONTROL 平台工具]**&#x200B;下展开&#x200B;**[!UICONTROL 应用程序]**。

1. 单击&#x200B;**[!UICONTROL 已安装的包]**。

   请注意，已安装&#x200B;**[!DNL Workfront]**&#x200B;包。

1. 单击&#x200B;**[!UICONTROL 旁边的]**&#x200B;配置&#x200B;**[!DNL Workfront]**。

1. 以系统管理员身份登录到[!DNL Workfront]。

   显示&#x200B;**[!UICONTROL 触发器]**&#x200B;页。

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. 单击&#x200B;**[!UICONTROL 新建触发器]**。
1. 从&#x200B;**[!UICONTROL [!DNL Salesforce]对象]**&#x200B;下拉菜单中，选择&#x200B;**[!UICONTROL Opportunity]**。

   这是必填字段。

1. （视情况而定）指定以下内容：

   1. 从&#x200B;**[!UICONTROL 舞台]**&#x200B;下拉菜单中，选择&#x200B;**[!UICONTROL 舞台]**。\

      当机会到达此处指定的[!UICONTROL 阶段]时，将在[!DNL Workfront]中创建项目。 这是必填字段。

   1. 在&#x200B;**[!UICONTROL Portfolio或项目群]**&#x200B;字段中，开始键入要将项目放置在[!DNL Workfront]中的Portfolio或项目群的名称，然后当该项目出现在列表中时将其选定。\

      如果未指定Portfolio或项目群，则在配置触发器时，将创建新项目并将其添加到登录到[!UICONTROL 的用户的]我拥有的项目[!DNL Workfront]列表中。 该用户也是新项目的项目所有者。

   1. 开始键入要与新[!DNL Workfront]项目关联的模板的名称，然后将其在列表中显示时选定。\

      这是必填字段。


      >[!NOTE]
      >
      >如果您在计划用于此集成的模板上指定了模板所有者，则该模板所有者将成为新项目的项目所有者。 根据该模板，新项目显示在新项目的所有者用户列表的[!UICONTROL 我拥有的项目]下。

   1. （可选）如果要为任何一个销售机会下销售的每种产品类型创建新项目，请选择&#x200B;**[!UICONTROL 为每个销售的产品类型创建新项目]字段**。
   1. （视情况而定）在&#x200B;**[!UICONTROL 产品]**&#x200B;下拉菜单中选择&#x200B;**[!UICONTROL 产品]**。

      这是必填字段。

   1. （视情况而定）开始键入要与新&#x200B;**[!UICONTROL 项目关联的]**&#x200B;模板[!DNL Workfront]的名称（如果指定的产品位于[!UICONTROL Opportunity]上）。 当它出现在列表中时将其选中。

      这是必填字段。

      在将新产品添加到[!DNL Salesforce]机会时创建的项目放在为该机会选择的同一Portfolio或项目中。

      >[!IMPORTANT]
      >
      >项目仅在[!UICONTROL Opportunity]上更新阶段时创建。 为更新暂存字段时指定的每个产品创建一个唯一项目，而不是为添加到[!UICONTROL Opportunities]中的产品创建唯一项目。

1. （可选）单击&#x200B;**[!UICONTROL 新建触发器]**。
1. （可选）从&#x200B;**[!UICONTROL [!DNL Salesforce]对象]**&#x200B;下拉菜单中，选择**帐户
**。

   这是必填字段。
1. （视情况而定）指定以下内容：

   1. 从&#x200B;**[!UICONTROL 类型]**&#x200B;下拉菜单中选择&#x200B;**[!UICONTROL 类型]**。

      当有任何**帐户时
**被指定为**&#x200B;[!UICONTROL 中此处指定的]&#x200B;**&#x200B;类型[!DNL Salesforce]，在&#x200B;**&#x200B;[!UICONTROL 中创建了]**&#x200B;项目[!DNL Workfront]。

      这是必填字段。

   1. （可选）开始在&#x200B;**[!UICONTROL Portfolio或项目]**&#x200B;字段中键入要将项目放置在&#x200B;**[!UICONTROL 中的]** Portfolio[!DNL Workfront]或&#x200B;**[!UICONTROL 项目]**&#x200B;的名称，然后当项目出现在列表中时将其选定。

      如果未指定Portfolio或项目群，则会创建新项目并将其添加到从&#x200B;**[!UICONTROL 登录到]**&#x200B;的用户的[!DNL Workfront]我拥有的项目[!DNL Salesforce]列表中。 用户还是新项目的项目所有者。

   1. 开始键入要与新&#x200B;**[!UICONTROL 项目关联的]**&#x200B;模板[!DNL Workfront]的名称，然后当它出现在列表中时将其选定。

      这是必填字段。

      >[!NOTE]
      >
      >如果您在计划用于此集成的模板上指定了模板所有者，则该模板所有者将成为新项目的项目所有者。 根据该模板，新项目显示在新项目的所有者用户列表的&#x200B;**[!UICONTROL 我拥有的项目]**&#x200B;下。

   ![salesforce_triggers_page_with_cleaned_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. 单击&#x200B;**[!UICONTROL 保存]**。

   现在，每当满足任何触发器时，都会生成[!DNL Workfront]项目。

### 了解项目名称 {#understanding-project-names}

根据生成项目的触发器，[!DNL Workfront]中的项目名称可能遵循以下任一模式：

* 如果项目是基于机会或帐户触发器创建的，则项目的名称为： *`<Salesforce object name>`： `<Project template name>` （通过[!DNL Salesforce]）*。
* 如果项目是基于同时包括添加新产品的机会触发器创建的，则项目的名称为： *`<Salesforce object name>`： `<Salesforce product name>` （通过[!DNL Salesforce]）*。

## 查看[!DNL Workfront]个项目

如果[!DNL Workfront]管理员已将[!DNL Workfront]部分添加到您的[!UICONTROL Opportunity]或帐户
页面布局，您可以看到在此分区的[!UICONTROL 项目]选项卡中自动创建的项目。\
有关将[!DNL Workfront]部分添加到[!UICONTROL Opportunity]或帐户的页面布局的详细信息
，请参阅[为 [!DNL Adobe Workfront] 用户配置 [!DNL Salesforce] 部分](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)。

您必须拥有[!DNL Workfront]帐户并登录到[!DNL Workfront]才能查看[!UICONTROL 项目]选项卡。

查看从[!UICONTROL 机会]或帐户创建的项目
：

1. 转到[!UICONTROL Opportunity]或帐户
.
1. 转到 **[!DNL Workfront]** 部分。

   >[!NOTE]
   >
   >根据[!DNL Workfront]管理员配置此部分的方式，它可能具有不同的名称。

1. 选择&#x200B;**[!UICONTROL 项目]**&#x200B;选项卡。

   此选项卡中列出了由定义的触发器创建的所有项目。 任何在[!DNL Salesforce]中拥有[!DNL Workfront]帐户并且可能有权在[!DNL Workfront]中查看这些项目的用户也可以在[!DNL Salesforce]中查看[!UICONTROL 机会]或帐户的这些项目
产生它们的因素。

   您可以查看有关该集成所创建项目的以下信息：

   * 项目名称
   * 参考号
   * 输入日期
   * 所有者的名称
   * 状态
   * 完成情况
   * 规划完成日期
   * 完成百分比

     在[!DNL Workfront]中更新此信息时，您可以看到此列表中更新的字段。

1. （可选）单击项目的名称以在Workfront中将其打开。
1. （可选）单击[!UICONTROL **[!UICONTROL 项目详细信息]**]区域或项目标题中的[!UICONTROL 转到Salesforce]以访问[!UICONTROL 机会]或帐户
项目的来源。 您的系统或组管理员必须将[!UICONTROL 集成]字段添加到您的布局模板中，才能在项目标头中找到该字段。

   >[!NOTE]
   >
   >[!UICONTROL 转到Salesforce]链接对可以查看该项目的所有[!DNL Workfront]用户可见。 您必须拥有[!DNL Salesforce]帐户才能转到生成项目的[!DNL Salesforce]机会或帐户。
