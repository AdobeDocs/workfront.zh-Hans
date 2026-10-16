---
title: 在构思空间中创建简报
description: 本文介绍了如何在构思空间中集思广益和制定策略以创建摘要。 您可以将完成的构思简报导出到文件或Workfront Planning以创建或更新记录。
feature: Workfront Planning
role: User, Admin
author: Alina
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: e209f8e5ada29b1c488fcfe42c13c6c9523a26bd
workflow-type: tm+mt
source-wordcount: '1621'
ht-degree: 1%
---

# 在构思空间中创建简报

<!--add to TOC and miniTOC-->

<span class="preview">此页面上的信息引用了尚未公开的功能。 它只能作为&#x200B;**构思空间Beta**&#x200B;程序的一部分提供。</span>

<span class="preview">有关详细信息，请参阅[Adobe Workfront规划构思空间入门](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)。</span>

{{planning-important-intro}}

使用创意空间（Adobe Workfront Planning的一项新功能），您可以将摘要转换为Planning记录或另存为外部文件。 导出的摘要可创建新记录或更新现有记录。

本文介绍了如何在构思空间中集思广益和制定策略以创建摘要。

您可以执行以下操作：

* 要创建或更新记录，请将完成的构思简报导出到Workfront Planning。

* 要在另一个应用程序中使用简介的信息，请将其导出为下列文件类型之一：

  * PDF
  * 字词
  * PowerPoint
  * PowerPoint模板

## 访问权限要求

+++ 展开以查看本文中各项功能的访问要求。 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 包</p></td> 
   <td> 
<ul> 
<li><p>带规划包的任何Workfront或工作流</p></li>
<!--
Add this at GA - not available in beta:
Or
<li><p>Any Planning package when purchased as a standalone product</p></li>
-->
</ul>
   </td> 
<!--
<tr> 
<td role="rowheader"><p>Additional products</p></td> 
<td><ul>
<li><p>Adobe GenStudio for Performance Marketing</p></li>
<li><p>Adobe Customer Journey Analytics</p></li>
</ul>
</td> 
</tr> 
-->
  <tr> 
   <td role="rowheader"><p>Adobe工作流许可证</p></td> 
   <td><p>标准</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe计划许可证</p></td> 
   <td><p>标准</p>
   </td> 
  </tr>  
<tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> 
   <ul>
   <li><p>当您同时具有Workflow和Planning包时，必须将工作流和Planning许可证类型添加到访问级别</p>   </li>
   <li><p>必须取消选择访问级别中的禁用创意空间设置</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td> <p>为要添加记录的工作区和记录类型提供或更高权限 </p>
      <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
      <!--
      not available right now:
      <p>View permissions to Workfront objects to add them to briefs </p>
      -->
      <p>创意空间上的编辑器权限以创建摘要</p>
   </td> 
  </tr>  
    <!--
    <tr> 
    <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
    <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
    <li>GenStudio System Manager to access Activations and Events</li></ul>
    For information, see <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
    </p>
    </td> 
    </tr> 
    -->
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++  

## 创建构思空间简述

您可以创建摘要以创建或编辑Planning记录，或者创建可导出到其他应用程序的文件。

1. 使用Planning登录（Co-worker已打开），并执行以下操作之一：

   * 转到&#x200B;**主菜单** > **构思空间**
   * 转到&#x200B;**主菜单** > **规划** >单击工作区>单击记录类型> **新记录** > **开始创意空间**

     有关使用构思空间创建记录的详细信息，请参阅[从构思空间简述创建计划记录](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)。
   * 转到&#x200B;**主菜单** > **规划** >单击工作区>单击记录类型>单击现有记录> **在创意空间中打开**

   构思空间打开，新构思的标题默认遵循以下格式：

   `catalyze-canvas-< number > - Month date, year at time` <!--submitted bug to change the default name to "Untitled ideation"-->

   如果从现有记录中打开构思，则构思名称与记录的名称匹配。

1. （推荐）单击构思的名称以更改名称。

1. （有条件，可选）要打开另一个现有的构思空间，请单击构思名称右侧的下拉菜单，按名称搜索构思，然后在构思显示在列表中时单击该构思。

1. 当&#x200B;**构思空间**&#x200B;打开时，CX Coworker会在右侧打开。 使用Co-worker提示符描述要创建的简介类型。

   例如，键入“Create a back-to-school campaign for K-12 student to run through the month of 8月，for parents and teachers in the US”。  要使简报尽可能完整，请尽可能指明可用于何种营销活动、时间表、利益相关者、批准检查点和其他详细信息的信息。

1. 单击Enter。

1. 回答同事的问题以继续构思，然后单击&#x200B;**提交**

   或

   单击&#x200B;**跳过调查表**&#x200B;跳过其他问题。

1. （视情况而定）当同事为创意内容创建卡片时，回答&#x200B;**是**。

   信息卡会添加到创意空间，您可以查看每个信息卡的来源并决定要将哪个信息卡添加到您的摘要。

1. 单击&#x200B;**搜索**&#x200B;图标![搜索图标](assets/search-icon.png)以搜索构思空间中的项目，然后单击该图标在列表中显示时导航到它。

1. （可选）单击每张卡片底部的&#x200B;**源**&#x200B;以了解从何处收集信息。

   可以从Workfront Planning或Web导入信息。

   您还可以单击空间右上角的&#x200B;**源**&#x200B;图标![源图标](assets/sources-icon.png)以显示空间中所有卡片的源列表。
1. （可选）单击共享空间右上角的&#x200B;**评论** ![评论图标](assets/comments-icon.png)，然后单击&#x200B;**@**&#x200B;标记其他人在共享空间内开始头脑风暴。

   用户将收到有关标记的电子邮件通知。
1. （可选）单击评论卡片中的&#x200B;**筛选器**&#x200B;图标![](assets/filter-comments-icon.png)以按以下条件筛选评论：

   * 审阅者
   * 添加评论的时间
   * 状态（评论已解决或尚未处理）
   * 未读（仅显示未读注释）
1. （可选）使用信息卡上的&#x200B;**向上缩略图**&#x200B;或&#x200B;**向下缩略图**&#x200B;图标![向上缩略图或向下缩略图图标](assets/thumbs-up-and-down-icons.png)对信息卡上的信息的准确性提供反馈。
1. 单击一张信息卡或单击包含所有信息卡的框架，然后单击&#x200B;**添加到简报**&#x200B;以将其信息添加到简报。

   Workfront会将每条信息与其找到的最可能存储它的字段进行匹配。

   例如，时间线添加到日期类型字段，说明添加到段落类型字段。

1. （视情况而定）单击信息卡，然后单击&#x200B;**向人工智能提问……**，以在将信息添加到简介之前获取有关下一步的想法。 答案取决于每张信息卡的上下文。
1. 单击位于构思空间左上角的&#x200B;**添加文档**&#x200B;图标![添加文档图标](assets/add-documents-in-ideation-space.png)以将文档上载到空间。 您可以添加新的文档或以前已添加到空间的文档。

   >[!TIP]
   >
   >必须启用“文档”设置才能访问文档并将文档上传到空间。
   >有关信息，请参阅本文中的[配置构思空间](#configure-the-ideation-space)部分。
   > 
1. 单击&#x200B;**添加WF分类卡**&#x200B;图标![从Workfront Planning添加](assets/add-from-wf-planning-on-ideations-space.png) <!--asked to change this tooltip-->并选择连接的记录类型，然后从每种类型中选择一条记录，将该记录的信息添加到您选择的记录类型中。

   将为您选择添加到空间的记录创建一张信息卡。 记录类型显示在记录卡片的左上角。

   >[!TIP]
   >
   >从主菜单访问构思空间时，**添加WF分类卡**&#x200B;图标<!--check UI name-->不可用，并且摘要未连接到Planning记录。

1. （可选）单击连接的记录卡上的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**在Workfront中查看**。

   记录详细信息页面将在Workfront Planning的另一个浏览器选项卡中打开。
1. （可选）选择构思框架或卡片，单击&#x200B;**删除**&#x200B;图标，然后单击&#x200B;**删除**&#x200B;以进行确认。 卡从构思空间中移除。

   当您删除与存储的文档或记录对应的信息卡时，项目会从构思空间中删除，但会保留在各自的应用程序中。

1. （可选）随时使用右下角的&#x200B;**向同事询问任何内容**&#x200B;框优化您的想法。

   例如，为特定信息卡键入`regenerate`以使AI使用更新的上下文重做该信息卡。 构思空间重新运行其推理步骤（搜索、合成、引证）并更新受影响的卡片。

1. （可选）单击任何构思卡片组中的其中一个紫色连接器，然后单击&#x200B;**复制完整提示**&#x200B;图标以将生成该卡的提示复制到剪贴板，然后将其粘贴到同事提示框中。

   ![复制到提示栏图标](assets/copy-to-prompt-bar-icon-highlighted.png)

1. （可选）单击创意空间顶部的&#x200B;**撤消**&#x200B;或&#x200B;**重做**&#x200B;图标![撤消和重做图标](assets/undo-redo-icons.png)以取消或撤消操作。
1. 缩小以查看全貌：您的原始营销活动目标、所有包含引文的AI生成的概念卡、其他文档、您已拉入的实际Workfront Planning记录（产品、角色等）。 左下角的&#x200B;**Brief**&#x200B;摘要卡将所有这些内容拉在一起。

1. 单击左下角的摘要预览图像并查看摘要，然后单击以下选项之一：

   * **导出到文件**。 您可以将简介导出到以下文件类型：

     * PDF
     * 字词
     * PowerPoint（带或不带模板）
   * **导出到Workfront计划**。 导出将覆盖Planning记录中与构思对应的所有现有字段数据。

   >[!TIP]
   >
   >从主菜单访问构思空间时，**导出到Workfront Planning**&#x200B;将灰显，并且摘要未连接到Planning记录。

   此操作将完成记录或文件的创建，并包含附加信息。 如果从现有记录开始，则摘要中的信息将添加到记录中。 如果您从新记录开始，则使用简介中的信息创建记录。

   有关使用摘要更新Planning记录的更多信息，请参阅[从创意空间摘要创建Planning记录](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)一文中的“关于使用创意空间创建记录的注意事项注意事项”部分。


## 配置构思空间

创意空间有一些控件，用于配置您在屏幕上看到的内容，并帮助您导航该空间。

1. 单击&#x200B;**设置**&#x200B;图标![设置](assets/setting-icon.png)以控制AI从何处提取信息，然后从以下&#x200B;**Source类型**&#x200B;中进行选择：

   * **文档** — 已上载到所选空间的文档
   * **Web搜索** — 外部Web研究
   <!--
     **CJA** — Adobe Customer Journey Analytics
    -->
1. 单击&#x200B;**保存**。

1. 单击&#x200B;**帮助**&#x200B;图标左侧的&#x200B;**缩放级别**&#x200B;下拉图标或&#x200B;**帮助**&#x200B;图标![帮助图标](assets/more-information-icon.png)以选择一个选项，或查看可用于导航构思空间或选择其他缩放值的键盘快捷键。

   从以下缩放级别中选择：

   * 缩放到100%
   * 缩放到200%
   * 缩放以适合

   或者使用以下快捷方式之一在页面上导航：

   | 操作 | 快捷键 |
   | --- | --- |
   | 放大/缩小 | Ctrl/⌘ + / − |
   | 缩放以适应/适应选择 | — |
   | 缩放到光标 | Ctrl/⌘ +滚动 |
   | 平移画布 | 按住空格+拖动 |
   | 显示/隐藏点网格 | G |



<!--

    Once opened, the Ideation space agent goes through the following steps:

    1. **Data ingestion and synthesis**:  Pulls relevant information from connected sources. For example: 
    
        * Existing record types or the existing record type that you started from. 
        * Recent documents you might have uploaded in the ideation space. 
        * Web information that matches your prompt criteria.

            >[!TIP]
            >
            >The Web search setting must be turned on for AI to be able to look for information on the web.  
            >For information, see the section [Configure the Ideation space](#configure-the-ideation-space)in this article.
            >
    1. **Audience definition**: Identifies or recommends target audience parameters based on historical patterns
    1. **Strategy framing**: Structures the strategic narrative for the campaign
    1. **Messaging and concept ideation**: Generates initial message options and creative concept directions
    1. **Brief generation and planning handoff**: Produces a structured brief that feeds back into the Workfront Planning workspace

        When the Ideation agent finishes the process of collecting all the information, the following things occur: 
    
        * Five cards are created and are organized by relevant and like-information. 

            The cards are titled using various steps in the creation of the requested record, for easy recognition. 
    
            For example, they could be named:

            * Plan
            * Timeline
            * Segments
            * Mechanics  
            * Messaging 

        The cards titles are custom to each card in the ideation. 

        * The cards are placed inside the same frame indicating this is the result of one ideation. 

        * A brief is created and displays in a preview image in the lower-left corner of the Ideation space. <!
    
        The brief contains suggested fields that the system considers pertinent to the ideas you are exploring. 
-->






