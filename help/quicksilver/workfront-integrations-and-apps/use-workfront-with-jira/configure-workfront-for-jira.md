---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 配置 [!DNL Adobe Workfront for Jira]
description: 您可以使用 [!DNL Adobe Workfront for Jira] 来集成 [!DNL Jira] 和 [!DNL Workfront] 系统。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: b1b55b8046aa771abb2cceda333940ccf827356a
workflow-type: tm+mt
source-wordcount: '2454'
ht-degree: 0%

---

# 配置[!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->


>[!IMPORTANT]
>
>为了提供更稳定和可扩展的集成，我们正在使用Workfront自动化与集成(Fusion)转向一种现代、灵活的集成方法。 在此过渡过程中，Workfront for Jira集成在&#x200B;**2026年2月28日**&#x200B;后不可用。
>
>为了满足贵组织与Jira的集成需求，我们建议使用Workfront自动化和集成。
>
>有关Workfront自动化和集成的概述，请参阅[Adobe Workfront Fusion概述](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>有关Jira的Workfront自动化和集成模块的特定功能的信息，请参阅[Jira软件模块](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules)。

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

您可以使用[!DNL Adobe Workfront for Jira]来集成[!DNL Jira]和[!DNL Workfront]系统。

安装加载项后，您可以定义在创建[!DNL Jira]工作项时自动创建[!DNL Workfront]问题的工作流。 两个应用程序中的项目会相互链接，并且其中的一些信息会在两个系统中自动更新。

[!DNL Workfront]和[!DNL Jira]中的所有用户都可从此集成中受益。 他们只需要许可证就可以使用他们最常使用的系统，而不需要许可证就可以同时使用两个系统。

此加载项可用于[!UICONTROL 软件的]服务器[!UICONTROL 和]OnDemand[!UICONTROL &#x200B; （或]云[!DNL Jira]）版本。

有关[!DNL Jira]当前支持的[!DNL Workfront for Jira]版本的列表，请参阅[[!DNL Workfront for Jira]上的](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) [!DNL Atlassian Marketplace]。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td><p>任何</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准 </p>
       <p>规划 </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Jira访问</td> 
   <td> <p>系统管理员访问权限</p> <p>重要信息：我们建议您在Jira和Workfront中创建单独的系统管理员帐户以专门用于此集成，而不是使用可能附加到用户的现有帐户。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在配置[!DNL Workfront for Jira]之前，您必须：

* 安装[!DNL Workfront for Jira]。
有关安装[!DNL Workfront for Jira]的说明，请参阅[安装 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)。

## 配置[!DNL Workfront for Jira]

通过配置[!DNL Workfront for Jira]，您可以：

* 定义将在创建[!DNL Jira]项时创建[!DNL Workfront]项的触发器。
* 指定在[!DNL Jira]和[!DNL Workfront]之间链接的项之间应同步的字段。

>[!NOTE]
>
>* 在您的[!DNL Workfront for Jira]环境中配置[!DNL Jira]后，所有[!DNL Jira]用户都会看到针对所有[!DNL Workfront]项目的[!DNL Jira]右侧面板。 该面板包含有关可能从[!DNL Workfront]链接的项的信息，或指定没有[!DNL Workfront]项链接到[!DNL Jira]项。
>* 使用[!DNL Jira Server]安装时，只有与标识为Workfront集成触发器的项目关联的问题才会显示Workfront面板。 有关为[!DNL Workfront to Jira]工作流设置触发器的详细信息，请参阅[配置触发器以自动链接介于 [!DNL Jira] 和 [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront)之间的项目。
>

要配置[!DNL Workfront for Jira]：

1. 以[!DNL Jira]管理员身份登录[!DNL Jira]。
1. 在主&#x200B;**[!UICONTROL 菜单中单击]**&#x200B;设置[!DNL Jira]。
1. 单击&#x200B;**[!UICONTROL 加载项]**，然后单击&#x200B;**[!UICONTROL 管理加载项]**。

1. 展开&#x200B;**[!DNL Workfront]**&#x200B;加载项。
1. 单击&#x200B;**[!UICONTROL 配置]**。
1. 按照提示登录[!DNL Workfront]。

   >[!NOTE]
   >
   >用户必须在`apiKey`Workfront[!UICONTROL 中具有有效的]才能创建成功的连接。

   您必须以[!DNL Workfront]管理员身份登录到[!DNL Workfront]才能继续配置。

   >[!NOTE]
   >
   >* [!UICONTROL Workfront]使用OAuth 2.0连接到[!DNL Jira]，该标准由大多数基于Web的集成用于用户身份验证和授权。
   >* 当系统提示您输入[!DNL Workfront]帐户的域时，请使用此格式键入该域： *您的公司&#39;sDomain.my.workfront.com*。 您公司的域通常是您公司的名称。
   >* 在[!DNL Workfront]管理员为此集成启用增强身份验证之前，该身份验证不可用。

1. 在Jira中，选择&#x200B;**[!UICONTROL 触发器]**&#x200B;选项卡，以便在创建新[!DNL Jira]项时配置自动创建[!DNL Workfront]项。

   有关将Workfront的触发器设置为[!DNL Jira]工作流的详细信息，请参阅[配置触发器以自动链接介于 [!DNL Jira] 和 [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront)之间的项目。

1. 选择&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡以配置链接的[!DNL Jira]和[!DNL Workfront]项之间的字段同步。

   有关设置[!DNL Jira]和[!DNL Workfront]之间的字段同步的详细信息，请参阅[配置 [!DNL Jira] 和 [!DNL Workfront] 项之间的字段同步](#configure-field-synchronization-between-jira-and-workfront-items)。

   >[!NOTE]
   >
   >定义两个应用程序之间的触发器和字段同步后，任何可以创建任务或问题的[!DNL Workfront]用户都可能会触发在[!DNL Jira]中创建项目。 如果所创建项目的条件与[!DNL Jira]中的触发器匹配，则用户可以创建项目，即使用户没有[!DNL Jira]许可证。 此外，任何[!DNL Jira]用户都可以立即开始处理[!DNL Jira]项目，并且他们的更新在[!DNL Workfront]中可见，而无需他们具有[!DNL Workfront]许可证。 [!DNL Workfront]中的任何更新也可在[!DNL Jira]项中看到。

1. （可选）选择&#x200B;**[!UICONTROL 活动日志]**&#x200B;选项卡以查看集成期间可能发生的任何错误。

   有关[!UICONTROL 活动日志]的详细信息，请参阅[查看 [!DNL Jira] [!UICONTROL 活动日志]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md)。

## 配置触发器以自动链接[!DNL Jira]和[!DNL Workfront]之间的项目

作为[!DNL Jira]系统管理员，您可以定义在[!DNL Jira]中的项满足特定条件时，在[!DNL Workfront]中自动创建问题的触发器。

>[!NOTE]
>
>集成最多可能需要10分钟才能在[!DNL Jira]中创建新问题。

在创建[!DNL Jira]项时配置触发创建[!DNL Workfront]项时，请考虑以下事项：

* 该集成是单向的：您只能触发您在[!DNL Workfront]中创建的项以便在[!DNL Jira]中自动创建。 您无法触发您在[!DNL Jira]中创建的项以在[!DNL Workfront]中自动创建。
* 您可以触发的触发器数量没有限制。
* 如果在[!DNL Workfront]中创建的项与多个触发器匹配，则在[!DNL Jira]中只创建一个项。 该项根据第一个触发器在[!DNL Jira]中创建（按照它们在[!DNL Jira]中定义的顺序）。 所有其他触发器将被忽略。
* [!DNL Workfront]中只能有一个项目链接到Jira中的一个项目。 您永远不能将一个[!DNL Workfront]项目链接到多个[!DNL Jira]问题，或将一个[!DNL Jira]问题链接到多个[!DNL Workfront]项目。

要配置触发器以在[!DNL Jira]中自动创建项目，请执行以下操作：

1. 以系统管理员身份登录到[!DNL Jira]。
1. 在主&#x200B;**[!UICONTROL 菜单中单击]**&#x200B;设置[!DNL Jira]。
1. 单击&#x200B;**[!UICONTROL 插件]**，然后单击&#x200B;**[!UICONTROL 管理插件]**。
1. 展开&#x200B;**[!DNL Workfront]**&#x200B;加载项。
1. 单击&#x200B;**[!UICONTROL 配置]**。
1. 以系统管理员身份登录到[!DNL Workfront]。

   在Jira中，默认选择&#x200B;**[!UICONTROL 触发器]**&#x200B;选项卡。

1. 单击&#x200B;**[!UICONTROL 添加触发器]**&#x200B;以添加新触发器。
1. 在&#x200B;**[!UICONTROL Workfront团队/用户/角色]**&#x200B;字段中，指定[!DNL Workfront]团队、用户或工作角色的名称，然后单击以将其在列表中显示。

   >[!NOTE]
   >
   >同一团队、用户或角色不能有多个触发器。

   当有人创建任务或问题并将其分配给其中一个实体时，问题会在[!DNL [!DNL Jira]]中自动创建。

1. 在&#x200B;**[!UICONTROL [!DNL Jira]项目]**&#x200B;字段中，开始输入[!DNL Jira]项目的名称，然后单击以将其在列表中显示。

   创建[!DNL Jira]问题后，该问题将放置到您在此处选择的项目上。

1. 从下拉菜单中选择&#x200B;**I[!UICONTROL 问题类型]**。

   此表示当满足此触发器的条件时，根据[!DNL Jira]中该特定项目的设置在[!DNL Jira]中创建的问题类型。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   使用此配置，每次[!DNL Workfront]用户创建与指定触发器匹配的项时，[!DNL Jira]中都会创建一个新问题。

## 配置[!DNL Jira]和[!DNL Workfront]项之间的字段同步

作为[!DNL Jira]管理员，您可以定义哪些字段应该自动同步在[!DNL Workfront]和Jira之间链接的项目。 某些字段可以从[!DNL Workfront]同步到[!DNL Jira]项，而其他字段可以从Jira同步到Workfront。

要定义应在两个应用程序之间链接的项目上自动同步的字段，请执行以下操作：

1. 以Jira管理员身份登录[!DNL Jira]。
1. 在主&#x200B;**[!UICONTROL 菜单中单击]**&#x200B;设置[!DNL Jira]。
1. 单击&#x200B;**[!UICONTROL 插件]**，然后单击&#x200B;**[!UICONTROL 管理插件]**。
1. 展开&#x200B;**[!DNL Workfront]**&#x200B;加载项。
1. 单击&#x200B;**[!UICONTROL 配置]**。
1. 以Workfront管理员身份登录到[!DNL Workfront]。
1. 在Jira中，单击&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡。
1. 在&#x200B;**[!UICONTROL 从Workfront同步到Jira]**&#x200B;部分中，选择在Workfront中更新时要在[!DNL Jira]中更新的字段。

   1. 选择以下任何与字段同步的频率：

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL On Creation]</td>
              <td>在Workfront中创建项时，您指定的字段会在链接的Workfront和[!DNL Jira]项之间同步。</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>在Workfront中更新字段时，您指定的字段会在链接的Workfront和[!DNL Jira]项之间同步。 </td>
          </tr>
          <tr>
              <td>[!UICONTROL 从不]</td>
              <td>您指定的字段从不在链接的[!DNL Workfront]和[!DNL Jira]项之间同步。 [!DNL Jira]中没有指示该字段已在[!DNL Workfront]中更新。 </td>
          </tr>
      </table>

   1. 选择以下任一选项以同步从[!DNL Workfront]到[!DNL Jira]的字段：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL 名称]</td>
         <td><p>[!DNL Workfront]中任务或问题的名称将成为它在[!DNL Jira]中链接到的问题的名称。</p><p>注意：在[!DNL Jira]中自动创建新项目时，[!DNL Workfront]名称始终在[!DNL Jira]项目上更新，无论是否在此处启用此字段。 当[!DNL Jira]项手动链接到[!DNL Workfront]项时，当您选择[!DNL Workfront]始终[!DNL Jira]同步此字段时，<strong>项的名称仅在</strong>中更新。 有关手动或自动链接项目的详细信息，请参阅<a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">链接介于[!DNL Adobe Workfront]和[!DNL Jira]</a>之间的项目。</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 描述]</td>
         <td>[!DNL Workfront]中任务或问题的描述将成为它在[!DNL Jira]中链接到的问题的描述。</td>
        </tr>
        <tr>
         <td role="rowheader">文档</td>
         <td><p>附加到[!DNL Workfront]中任务或问题的文档也附加到Jira中与之链接的问题。 来自[!DNL Workfront]的新文档版本将作为单独的文档添加到Jira中，并附加有<i>_v&lt;版本号&gt;</i>以指示Workfront中的编号版本。 </p><p>例如，如果[!DNL Workfront]中文档的名称为<strong>Main Ad</strong>，而您在[!DNL Workfront]中为其添加了新版本，则新版本将作为名称为[!DNL Jira]Main Ad_v2<strong>的新文档传输到</strong>。</p><p>重要提示： <p>同步文档时，请考虑以下事项：</p>
           <ul>
            <li><p>大于5MB的文档不会同步。 如果文档同步因文档太大而失败，则活动日志中会记录一个错误。 </p><p>有关活动日志的详细信息，请参阅<a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">查看Jira活动日志</a>。</p></li>
            <li><p>链接到来自外部服务器的任务和问题的文档未传输到[!DNL Jira]项。 只有直接在任务中上传的文档或[!DNL Workfront]中的问题才会传输到[!DNL Jira]中的链接问题。</p></li>
            <li><p>要从文档创建验证，必须在[!DNL Workfront]中生成验证。 </p><p>有关生成校对的更多信息，请参阅<a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">为文档创建校对</a>中的<a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">为现有文档创建校对</a>。<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 计划完成日期]</td>
         <td><p>[!DNL Workfront]中任务或问题的[!UICONTROL 规划完成日期]将变为[!DNL Jira]中链接到的问题的[!UICONTROL 到期日期]。</p><p>注意：请确保在<strong>个问题上显示</strong>[!UICONTROL 到期日期][!DNL Jira]，以便同步该值。</p></td>
        </tr>
       </tbody>
      </table>

1. 在&#x200B;**[!UICONTROL 从[!DNL Jira]同步到[!DNL Workfront]]**&#x200B;分区中，选择在[!DNL Workfront]中更新时要在[!DNL Jira]中更新的字段。

   1. 选择以下任何与字段同步的频率：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>在[!DNL Workfront]中更新字段时，您指定的字段始终在链接的[!DNL Jira]和[!DNL Jira]项之间同步。 </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 从不]</td>
         <td><p>您指定的字段从不在链接的[!DNL Workfront]和[!DNL Jira]项之间同步。 [!DNL Workfront]中没有指示该字段已在[!DNL Jira]中更新。 </p><p>注意：当您选择“从不”时，仍然可以从[!DNL Workfront]问题左侧[!DNL Jira]面板的[!DNL Workfront]手动更新[!DNL Jira]字段。 这些更新仅显示在[!DNL Workfront]和[!DNL Jira]中的[!DNL Workfront]项中，而不显示在[!DNL Jira]项中。</p></td>
        </tr>
       </tbody>
      </table>

   1. 选择以同步从[!DNL Jira]到[!DNL Workfront]的以下任何字段：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL 状态]</td>
         <td>[!DNL Jira]中问题的[!UICONTROL 状态]将变为[!DNL Workfront]中链接到的任务或问题的[!UICONTROL 状态]。<br>有关[!DNL Workfront]状态的详细信息，请参阅<a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">创建或编辑状态</a>。</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 被分派人]</td>
         <td><p>[!DNL Jira]中问题的[!UICONTROL 任务接受者]成为[!DNL Workfront]中链接到的任务或问题的[!UICONTROL 任务接受者]。</p><p>重要提示：当您将[!DNL Jira]中的项分配给没有[!DNL Workfront]帐户的用户时，只有当[!DNL Workfront]用户没有<strong>帐户[!DNL Workfront]的[!DNL Jira]在[!DNL Workfront]中自动创建用户设置为</strong>[!UICONTROL Always]<strong>时，集成才会在</strong>中创建新的活动用户。 此用户未占用[!DNL Workfront]许可证。 可将活动用户分配给[!DNL Workfront]中的工作项，但不能将其包含在更新中。 </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 附件]</td>
         <td>[!DNL Jira]中问题的附件也附加到[!DNL Workfront]中链接到的任务或问题。 </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comments]</td>
         <td><p>有关[!DNL Jira]问题的注释也会发布在[!UICONTROL 更新]区域的链接[!DNL Workfront]项上。 相反，[!UICONTROL 更新]区域中针对[!DNL Workfront]任务或问题的注释同步到[!DNL Jira]的链接问题的本机注释流。 </p><p>默认情况下设置为<strong>[!UICONTROL Always]</strong>。 如果在此选择<strong>[!UICONTROL Never]</strong>，则仍可在[!DNL Workfront]或[!DNL Jira]中对链接项手动发布评论。</p></td>
        </tr>
       </tbody>
      </table>

1. 在&#x200B;**[!UICONTROL OTHER]**&#x200B;部分中，选择应在链接项之间更新的其他字段。

   1. 选择一个选项，以确定您指定的字段&#x200B;**[!UICONTROL 始终]**&#x200B;还是&#x200B;**[!UICONTROL 从不]**&#x200B;在[!DNL Jira]或[!DNL Workfront]中进行更新（修改时）。

   1. 从以下字段和更新中进行选择：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">&lbrack;！UICONTROL在[!DNL Workfront]的右侧面板中复制[!DNL Jira]自定义数据</td>
         <td><p>在[!DNL Workfront]右侧面板中显示项目的[!DNL Workfront]自定义数据。</p><p>注意：自定义表单分区显示在[!DNL Workfront]右侧面板中，其访问级别为[!DNL Workfront]系统管理员。</p></td>
        </tr>
        <tr>
         <td role="rowheader">&lbrack;！UICONTROL复制[!DNL Workfront]中右侧面板的[!DNL Jira]优先级</td>
         <td>在[!DNL Workfront]右侧面板中显示项目的[!DNL Workfront]优先级。</td>
        </tr>
        <tr>
         <td role="rowheader">&lbrack;！UICONTROL在[!DNL Workfront]更新选项卡中添加有关[!DNL Jira]中到期日期更改的更新</td>
         <td>当链接的[!DNL Workfront]项中的[!UICONTROL 截止日期]发生更改时，在[!DNL Jira]项的[!UICONTROL 更新]选项卡中添加注释。</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 如果[!DNL Workfront]用户没有[!DNL Jira]帐户，则在[!DNL Workfront]中自动创建用户]</td>
         <td><p>存在以下情况：</p>
          <ul>
           <li>当您选择<strong>[!UICONTROL Always]</strong>时，您可以启用集成，以便在每次没有[!DNL Jira]帐户的[!DNL Workfront]用户对链接的[!DNL Jira]问题执行以下操作，创建新的Workfront用户：
            <ul>
             <li>已分派到[!DNL Jira]问题</li>
             <li><p>将时间记录到[!DNL Jira]问题</p><p>此新用户未占用[!DNL Workfront]许可证。 默认设置为“始终”。 在[!DNL Workfront]中通过这种方式创建的用户在名称中添加了“[!UICONTROL Jira]”。</p></li>
            </ul></li>
           <li>选择<strong>[!UICONTROL Never]</strong>时，会发生以下情况：
            <ul>
             <li>在[!DNL Jira]项中看不到任何[!DNL Workfront]分配。 在这种情况下，只有在[!DNL Workfront]中进行的分配会显示在[!DNL Workfront]项中。</li>
             <li>没有[!DNL Jira]帐户的用户登录到链接的[!DNL Workfront]问题的时间不会自动传输到链接的[!DNL Workfront]项目。 您仍然可以在[!DNL Workfront]问题的右侧面板中的[!DNL Jira]项上记录时间。</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. 单击&#x200B;**[!UICONTROL 保存]**。

   现在，每次用户更新此配置中针对[!DNL Jira]或[!DNL Workfront]中的项指定的任何字段时，另一个应用程序中的链接项也会更新。

## 故障排除

### 无法在[!DNL Jira]中创建项目，因为未能找到标记为“[!UICONTROL ”的触发器字段]”

#### 问题

当[!DNL Workfront for Jira]应用程序发生错误时，[!DNL Workfront]将禁用触发器以防止进一步的复杂性。 禁用这些触发器后，它们显示为“[!UICONTROL 找不到]”。

#### 解决方案

找到禁用触发器的错误。 您可以在[!DNL Workfront for Jira] [!UICONTROL 活动日志]中找到该错误。

导致此行为的最常见原因是错误&#39;&#39;[!UICONTROL 无法设置字段&#39;duedate&#39;。 它不在相应的屏幕上，或者未知。]”

此错误表示您正在尝试将&quot;[!UICONTROL 计划完成日期]&quot;从[!DNL Workfront]同步到[!DNL Jira]。 为此，您必须确保您的[!DNL Jira]对象具有一个名为“[!UICONTROL 到期日期]”的字段。 如果他们没有此字段，[!DNL Workfront]将无法从[!DNL Workfront]同步计划完成日期，并禁用您的触发器。

要解决此错误，请尝试以下操作之一：

* 要求您的[!DNL Jira]管理员更新受影响的[!DNL Jira]对象，以确保它们具有到期日期字段。
* 在Workfront [!DNL Workfront]设置[!UICONTROL 页面中禁用]计划完成日期的同步。
