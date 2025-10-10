---
title: 项目运行状况概述
content-type: reference
description: 项目运行状况功能利用AI Assistant的强大功能即时为您提供项目执行情况的评估。
author: Jenny
feature: Get Started with Workfront
exl-id: e4d200c6-7f35-4919-96d3-2880a655ed62
source-git-commit: d1ded406b8c4da975e2ff4d6825954cabd483ed2
workflow-type: tm+mt
source-wordcount: '1488'
ht-degree: 2%

---

# 项目运行状况概述

>[!IMPORTANT]
>
>项目运行状况功能目前仅适用于参与Beta阶段的用户。

Adobe Workfront的项目运行状况功能利用AI Assistant的强大功能即时为您提供对项目执行情况、哪些领域需要您关注以及如何避免可能会耗费您时间和资金的问题评估。

AI助手可以为以下对象生成项目运行状况评估：

* 单个项目
* 单个项目
* 多个项目

有关AI助手的详细信息，请参阅[AI助手概述](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)。

+++ 展开以查看访问要求。 
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划</p></td> 
   <td> 
<p>选择、Prime或Ultimate </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td> 
<p>标准</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td><p>管理员以管理项目运行状况配置 </p>
   <p>编辑以应用项目运行状况配置 </p>
     <p>查看以查看项目运行状况配置 </p>
  </td> 
  </tr>  
    </tr>  
</tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 注册Project Health测试版

为了利用项目健康，您的组织必须启用AI助手。

要为贵组织启用AI助手和项目运行状况，必须应用以下所有项：

* 贵组织必须已迁移到Adobe IMS (Identity Management System)。
* 您的组织必须具有Select、Prime或Ultimate Workfront计划
* 必须启用Adobe Unified Experience。
* Adobe必须有一个已签署的Adobe Gen AI协议文件。
* Workfront管理员必须为贵组织中的用户启用AI助手。 通过访问级别启用AI助手。
* 必须在设置>系统>首选项中的AI首选项部分选择启用AI和项目运行状况选项。

  ![AI首选项部分](assets/ai-preferences.png)

有关详细信息，请参阅[AI助手概述](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)和[配置系统首选项](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

## AI助手提示列表

下面是一个提示列表，您可以使用它请求AI评估为项目、项目群或帐户中的所有项目生成项目运行状况评估。

<table>
    <tr>
        <td><b>位置</b></td>
        <td><b>提示</b></td>
    </tr>
    <tr>
        <td>特定项目详细信息页面</td>
        <td><em>此项目的运行状况如何？</em></td>
    </tr>
    <tr>
        <td>Workfront中的任何页面 </td>
        <td><em>[PROJECT NAME]项目的运行状况如何？</em></td>
    </tr>
    <tr>
        <td>Workfront中的任何页面 </td>
        <td><em>我的项目运行状况如何？</em></td>
    </tr>
       <tr>
        <td>特定项目详细信息页面</td>
        <td><em>此计划的运行状况如何？</em></td>
    </tr>
       <tr>
        <td>Workfront中的任何页面 </td>
        <td><em>[计划名称]计划的运行状况如何？</em></td>
    </tr>
   </table>


## 项目和项目群完成情况列表

以下是生成项目运行状况评估时，AI助手将分配您的项目或项目群的可用条件。

<table>
    <tr>
        <td><b>项目完成情况</b></td>
        <td><b>项目进度状态</b></td>
        <td><b>项目完成情况因素</b></td>
    </tr>
    <tr>
        <td>准时</td>
        <td>当以下因素的平均风险级别处于健康阈值内时，将分配此分析。
        </td>
        <td> 
        <ul><li>范围蔓延</li>
        <li>缺少字段</li>
        <li>计划变更</li>
        <li>低估的工作</li>
        <li>项目进度</li>
        <li>逾期任务</li>
        <li>预算</li>
        </ul></td>
    </tr>
    <tr>
        <td>处于风险中</td>
        <td>当以下因素的平均风险水平刚好低于健康阈值时，即分配此分析。</td>
        <td>
        <ul><li>范围蔓延</li>
        <li>缺少字段</li>
        <li>计划变更</li>
        <li>低估的工作</li>
        <li>项目进度</li>
        <li>逾期任务</li>
        <li>预算</li>
        </ul></td>
    </tr>
    <tr>
        <td>存在问题</td>
        <td>当以下因素的平均风险级别低于健康阈值时，将分配此分析。</td>
        <td>
        <ul><li>范围蔓延</li>
        <li>缺少字段</li>
        <li>计划变更</li>
        <li>低估的工作</li>
        <li>项目进度</li>
        <li>逾期任务</li>
        <li>预算</li>
        </ul></td>
    </tr>
    </tr>
   </table>

## 管理项目运行状况配置

项目运行状况配置包含确定如何计算项目运行状况的特定标准。 创建配置后，您可以将其应用于项目。

>[!NOTE]
>
>您必须是系统管理员才能管理项目运行状况配置。

{{step-1-to-setup}}

1. 单击左侧面板中的&#x200B;**项目首选项**，然后在显示的下拉列表中选择&#x200B;**项目运行状况**。

1. 在页面的右上角，选择&#x200B;**新建配置**。

1. （可选）在配置详细信息页面上，将&#x200B;*无标题配置*&#x200B;替换为新的配置&#x200B;**名称**。

1. 在&#x200B;**要包括在项目运行状况中的因素**&#x200B;部分中，取消选择确定项目运行状况条件时不希望包括的任何因素：
   * **范围蠕变**：项目范围自启动以来扩展了多少。

   * **必填字段**：如果缺少任何必填字段（例如项目描述）。 这些必填字段决定项目完整性，并在&#x200B;**您要检查哪些字段的完整性？**&#x200B;配置部分如下。


   * **计划更改**：自项目启动以来，发生了多少次计划更改。

   * **任务估计**：估计任务工作的准确程度（例如，项目中当前没有逾期任务）。

   * **任务燃尽**：与项目时间线相比，项目工作的进度如何。

   * **超期任务**：当前已超过其到期日期的任务数。

   * **成本**：如果项目当前超出预算。

1. 在&#x200B;**中，您的项目何时正式开始？**&#x200B;部分中，从下拉列表中选择表示项目开始的事件。

1. 在&#x200B;**中，如何估计项目的工作范围？**&#x200B;部分中，选择哪个项目因子将随着项目范围的增加而增大。

1. 在&#x200B;**您要检查哪些字段的完整性？**&#x200B;部分中，选择一个或多个将被检查以确定项目完整性的字段。

   ![项目完整性字段](assets/project-completeness-fields.png)


1. 单击右上角的&#x200B;**保存**。

## 应用项目运行状况配置

管理员创建项目运行状况配置后，具有编辑权限的用户可以将其应用于项目。


{{step1-to-projects}}

1. 在&#x200B;**项目**&#x200B;页面上，选择一个项目。

1. 单击项目名称右侧的&#x200B;**更多**&#x200B;图标![更多图标](assets/more-icon.png)，然后选择&#x200B;**编辑**。 将打开&#x200B;**编辑项目**&#x200B;侧面板。

1. 在左侧面板中，选择&#x200B;**项目设置**。

1. 在&#x200B;**项目运行状况配置**&#x200B;字段中，选择要应用于此项目的配置。

   ![项目运行状况配置字段](assets/project-health-configurations.png)

1. 单击面板左下角的&#x200B;**保存**。

## 为项目或项目群生成项目运行状况评估

如果您具有项目或项目群的查看访问权限，则可以使用AI助手生成其项目运行状况评估。

如果您正在为项目生成评估，则可以在项目页面中完成评估，或者在询问助理项目执行情况的过程中引用项目名称。

如果您正在为项目生成评估，则可以在项目详细信息页面中执行该操作。

>[!NOTE]
>
>在项目启动之前，无法为项目生成项目运行状况评估。 您可以在项目设置中配置哪个事件触发项目开始。

有关详细信息，请参阅本文中的以下部分：[管理项目运行状况配置](#manage-project-health-configurations)。

1. 导航到要为其生成项目运行状况评估的项目或项目群。

1. 在项目/项目群详细信息页面上，单击屏幕右上角的&#x200B;**AI助手**&#x200B;图标![AI助手图标](assets/ai-assistant-icon.png)。 AI助手将打开。

1. 在&#x200B;**向我询问Workfront**&#x200B;字段中键入以下内容： *此项目的运行状况如何？*

   或

   在&#x200B;**向我询问Workfront**&#x200B;字段中键入以下内容： *此程序的运行状况如何？*

   >[!NOTE]
   >
   >如果您正在从Workfront中的其他页面访问AI助手，则可以键入&#x200B;*项目[项目名称]的运行状况如何？*&#x200B;或&#x200B;*程序[程序名称]的运行状况如何？* <br>
   >有关可输入的当前提示的完整列表，请参阅本文中的以下部分：[AI助手提示列表](#ai-assistant-prompts-list)。

1. 点击&#x200B;**发送**&#x200B;图标![发送图标](assets/send-icon.png)。 项目运行状况评估将生成并显示在面板中。 每个项目运行状况评估顶部都会显示一个徽章，反映项目的当前状态。

   ![项目运行状况评估](assets/health-assessment.png)

   如果您在为项目组合生成评估，将列出多个徽章，显示项目中每个项目的完成情况。 有关徽章标签的详细信息，请参阅本文中的以下部分：[项目和项目群条件列表](#project-and-program-conditions-list)。

1. （可选）单击其中一个评估点以展开其详细信息。

1. （可选）在展开的详细信息模式下，单击任务链接以打开任务详细信息。

   ![扩展的详细信息](assets/expanded-details.png)

1. 查看项目运行状况详细信息后，单击AI助手右上角的&#x200B;**关闭**&#x200B;图标![关闭图标](assets/close-icon.png)。

## 为多个项目生成项目运行状况评估

您可以为当前具有查看权限（或更高版本）的所有项目生成合并的项目运行状况评估。

仅当项目已启动时，项目才会包含在合并的项目运行状况评估中。 您可以在项目设置中配置哪个事件触发项目开始。 有关详细信息，请参阅本文中的以下部分：[管理项目运行状况配置](#manage-project-health-configurations)。

1. 单击屏幕右上角的&#x200B;**AI助手**&#x200B;图标![AI助手图标](assets/ai-assistant-icon.png)。 AI助手将打开。

1. 在&#x200B;**询问有关Workfront的信息**&#x200B;字段中键入以下内容： *我的项目的运行状况如何？*

   有关可输入的当前提示的完整列表，请参阅本文中的以下部分：[AI助手提示列表](#ai-assistant-prompts-list)。

1. 点击&#x200B;**发送**&#x200B;图标![发送图标](assets/send-icon.png)。 项目运行状况评估将生成并显示在面板中。

   ![多个项目评估](assets/multiple-projects-assessment.png)

   为多个项目生成评估时，AI Assistant会根据项目当前的执行方式将结果分组。

1. （可选）单击其中一个项目运行状况徽章以展开项目列表，然后选择特定项目的链接以转到该项目的详细信息页面。

1. 查看项目的运行状况详细信息后，单击AI助手右上角的&#x200B;**关闭**&#x200B;图标![关闭图标](assets/close-icon.png)以将其关闭。

<!--

## Build a Project Health table report in a Canvas Dashboard

>[!IMPORTANT]
>
>The Canvas Dashboards feature is currently only available for users participating in the beta stage. For more information, see [Canvas Dashboards beta information](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md). 

You can add a table report to a Canvas Dashboard in order to easily visualize your Project Health data in a table format.  

### Prerequisites 

You must create a dashboard before you can build a table report. 

For more, see [Create a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

### Build a Project Health table report 

There are many configuration options available for building a Project Health table report. In this section, we'll walk you through the process of creating one that displays the following columns: 

* **Name**: Contains the project name. 
* **Project Health Analysis**: Contains a summary of the Project Health assessment. 
* **Project Health Created At**: Contains the date/time when the Project Health assessment was last generated. 
* **Project Health Label**: Contains the project's label (e.g. On Target, At Risk, or In Trouble).

{{step1-to-dashboards}}

1. In the left panel, click **Canvas Dashboards**. 
1. In the upper-right corner, click **New Dashboard**. 
1. In the **Create dashboard** box, enter the dashboard's **Name** and **Description**. 
1. Click **Create**. 
1. In the **Add report** box, select **Create report**. 
1. On the left side, select **Table**. 
1. In the upper-right corner, click **Create report**. 
1. (Optional) Follow the steps below to configure the **Details** ![Details icon](assets/details-icon.png) section: 
    1. Enter a report **Name**. 
    1. Enter a report **Description**. 
1. Follow the steps below to configure the **Build table** ![Build table icon](assets/drilldown-column.png) section: 
    1. In the left panel, click the **Table columns** icon. 
    1. Click **Add column**, then select **Project** > **Name**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Health Analysis**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Created At**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Health Label**. 

1. Follow the steps below to configure the **Filter** ![Filter icon](assets/filter-icon.png) section: 
    1. In the left panel, click the **Filter** icon. 
    1. Select **Edit filter**. 
    1. Click **Add condition** and then specify the field you want to filter by and the modifier that defines what kind of condition the field must meet. The column appears in the preview section on the right.
    1. (Optional) Click **Add filter group** to add another set of filtering criteria. The default operator between the sets is AND. Click the operator to change it to OR. 

1. Follow the steps below to configure the **Drilldown Group Settings** ![Group settings](assets/drilldown-group-icon.png) section: 
    1. In the left panel, click the **Group Settings** icon. 
    1. Click the **Add grouping** button and then select the field you want to create as a grouping. The grouping column appears in the preview section on the right. 

1. Click **Save** to create the report.

-->
