---
title: 在构思空间中创建简报
description: 本文介绍了如何在构思空间中集思广益和制定策略以创建摘要。 您可以将完成的构思简报导出到文件或Workfront Planning以创建或更新记录。
feature: Workfront Planning
role: User, Admin
author: Alina
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 1%

---


# 在构思空间中创建简报

<!-- add to TOC and miniTOC-->

<span class="preview">此页面上的信息引用了尚未公开的功能。 它只能作为&#x200B;**构思空间Beta**&#x200B;程序的一部分提供。</span>

<span class="preview">有关详细信息，请参阅[Adobe Workfront规划构思空间入门](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)。</span>

{{planning-important-intro}}

使用Adobe Workfront Planning的新功能Ideation Space，您可以将简报转换为Planning记录。 导出的摘要可创建新记录或更新现有记录。

本文介绍了如何在构思空间中集思广益和制定策略以创建摘要。 要创建或更新记录，请将完成的构思简报导出到文件或Workfront Planning。

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
或
<li><p>作为独立产品购买时的任何Planning包</p></li></ul>
   </td>

<tr> 
   <td role="rowheader"><p>其他产品</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
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
      <p>查看对Workfront对象的权限以将其添加到摘要 <!--not sure if this is available--></p>
      <p>创意空间上的编辑器权限以创建摘要</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing用户角色</p></td> 
   <td><p><ul><li>用于访问营销活动、产品和角色的任何GenStudio用户角色</li>
   <li>用于访问激活的GenStudio系统管理器 <!--and Events--></li></ul>
   有关信息，请参阅<a href="https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">用户角色和权限</a>。 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++  

## 创建构思空间简述

1. 在Workfront Planning中开始，使用构思空间创建或编辑记录。

   有关详细信息，请参阅[从构思空间简述创建Planning记录](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)。
1. 当&#x200B;**构思空间**&#x200B;打开时，请使用提供的提示描述您要创建的简报类型。

   例如，键入“Create a back-to-school campaign for K-12 student to run through the month of 8月，for parents and teachers in the US”。  要使简报尽可能完整，请尽可能指明可用于何种活动、时间线、利益相关者和其他详细信息的信息。

1. 单击&#x200B;**开始构思**。

   打开后，构思空间代理将执行以下步骤：

   1. **数据摄取和合成**：从连接的源中提取相关信息。 例如：

      * 现有记录类型或您启动的现有记录类型。
      * 您可能在创意空间上载的最近文档。
      * 与提示条件匹配的Web信息。

        >[!TIP]
        >
        >必须启用Web搜索设置，AI才能在Web上查找信息。\
        >有关信息，请参阅本文中的[配置构思空间](#configure-the-ideation-space)部分。
        >
   1. **受众定义**：根据历史模式标识或推荐目标受众参数
   1. **战略框架**：构建营销活动的战略叙述
   1. **消息传递和概念构思**：生成初始消息选项和创意概念方向
   1. **Brief生成和规划移交**：生成结构化的摘要，以反馈到Workfront规划工作区

      当构思代理完成收集所有信息的过程时，会发生以下情况：

      * 将创建五张信息卡，并按相关信息或类似信息整理这些信息卡。

        这些卡片使用创建请求记录中的各种步骤进行标注，以便于识别。

        例如，可以将它们命名为：

        * 规划
        * 时间线
        * 区段
        * 力学
        * 消息

      卡片标题根据创意中的每个卡片进行自定义。

      * 卡片放在同一框架中，这表示这是一个构思的结果。

      * 将创建一个摘要，该摘要将显示在“构思”空间左下角的预览图像中。<!--add screen shot??-->

      该简介包含系统认为与您探索的想法相关的建议字段。

1. （可选）单击右上角的&#x200B;**帮助**&#x200B;图标![](assets/more-information-icon.png)以获取键盘快捷键列表，以帮助您在创意空间中进行导航。

1. （可选）单击每张卡片底部的&#x200B;**源**&#x200B;以了解从何处收集信息。

   可以从Workfront Planning或Web导入信息。
1. （可选）使用信息卡上的向上或向下缩略图标提供反馈。<!--is this still available??-->
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
   1. 单击&#x200B;**添加WF分类卡**&#x200B;图标![从Workfront Planning添加](assets/add-from-wf-planning-on-ideations-space.png) <!--send this tooltip to be revised-->并选择连接的记录类型，然后从每种类型中选择一条记录，将该记录的信息添加到您选择的记录类型中。

      将为您选择添加到空间的记录创建一张信息卡。 记录类型显示在记录卡片的左上角。
   1. （可选）单击&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**在Workfront中查看**。

      记录详细信息页面将在Workfront Planning的另一个浏览器选项卡中打开。
   1. （可选）选择构思框架或卡片，单击“删除”图标，然后单击“删除”以确认。 卡从构思空间中移除。

      当您删除与存储的文档或记录对应的信息卡时，项目会从构思空间中删除，但会保留在各自的应用程序中。

1. （可选）随时使用右下角的&#x200B;**询问任何内容**&#x200B;框来优化您的想法。

   例如，为特定信息卡键入`regenerate`以使AI使用更新的上下文重做该信息卡。 构思空间重新运行其推理步骤（搜索、合成、引证）并更新受影响的卡片。

1. （可选）在&#x200B;**询问任何内容**&#x200B;框中，询问新问题以开始新构思。

   空间重新运行其推理步骤后，将生成一组新的卡片。

1. （可选）单击任何构思卡片组中的其中一个紫色连接器，然后单击&#x200B;**复制到提示栏**&#x200B;图标以重新运行构思推理。

   ![复制到提示栏图标](assets/copy-to-prompt-bar-icon-highlighted.png)

1. （可选）单击页面顶部的&#x200B;**撤消**&#x200B;或&#x200B;**重做**&#x200B;图标![撤消和重做图标](assets/undo-redo-icons.png)以取消或撤消操作。
1. 缩小以查看全貌：您的原始营销活动目标、所有包含引文的AI生成的概念卡、其他文档、您已拉入的实际Workfront Planning记录（产品、角色等）。 左下角的&#x200B;**Brief**&#x200B;摘要卡将所有这些内容拉在一起。

1. 单击左下角的摘要预览图像并查看摘要，然后单击以下选项之一：

   * **导出到文件**。 您可以将简介导出到以下文件类型：

     * PDF
     * 字词
     * PowerPoint（带或不带模板）
   * **导出到Workfront计划**。 导出会覆盖Workfront Planning中记录的所有现有字段数据。

   此操作会完成使用附加信息创建记录，并将其添加到您最初选择的记录类型。

   有关使用摘要更新Planning记录的更多信息，请参阅[从创意空间摘要创建Planning记录](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)一文中的“关于使用创意空间创建记录的注意事项注意事项”部分。


## 配置构思空间

创意空间有一些控件，用于配置您在屏幕上看到的内容，并帮助您导航该空间。

1. 单击&#x200B;**设置**&#x200B;图标![设置](assets/setting-icon.png)以控制AI从何处提取信息，然后从以下&#x200B;**Source类型**&#x200B;中进行选择：

   * **文档** — 已上载到所选空间的文档
   * **Web搜索** — 外部Web研究
   * **CJA** — Adobe Customer Journey Analytics

1. 单击&#x200B;**保存**。

1. 单击&#x200B;**帮助**&#x200B;图标![帮助图标](assets/more-information-icon.png)可查看可用于导航构思空间或选择其他缩放值的键盘快捷键。

   从以下缩放级别中选择：

   * 缩放到100%
   * 缩放到200%
   * 缩放以适合

   或者使用以下快捷方式之一在页面上导航：

   | 操作 | 快捷键 |
   |---|---|
   | 放大/缩小 | Ctrl/⌘ + / − |
   | 缩放以适应/适应选择 | — |
   | 缩放到光标 | Ctrl/⌘ +滚动 |
   | 平移画布 | 按住空格+拖动 |
   | 显示/隐藏点网格 | G |

1. 单击“搜索”图标以搜索构思空间中的项目，然后在列表中显示时单击以导航到该构思空间。








