---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Adobe Workfront展示板模块
description: 您可以使用Adobe Workfront展示板连接器自动执行Workfront展示板中的流程，并将其连接到第三方应用程序和服务。
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
source-git-commit: db3f5b1e406d62fd0d3b99cb108ad824d1a32c24
workflow-type: tm+mt
source-wordcount: '2111'
ht-degree: 1%

---

# [!DNL Adobe Workfront] 展示板模块

>[!NOTE]
>
>此连接器当前处于Beta测试阶段。

Adobe Workfront展示板是一种灵活的工具，通过提供对包含列和卡片的共享展示板的访问，允许团队协作。

您可以使用Adobe Workfront展示板模块读取或更新记录，对Workfront展示板API进行API调用，或当展示板上发生操作时触发场景。

有关Workfront展示板的一般信息，请参阅 [展示板概述](/help/quicksilver/agile/boards-overview.md).

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td>
  <td> <p>任何</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td>
   <td> <p>新增：标准</p><p>或</p><p>当前： [！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证</td> 
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 对于工作自动化和集成]，[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).


## 先决条件

您必须先在Adobe Workfront中配置讨论区，然后才能连接到该讨论区。

## 创建与Workfront展示板的连接

>[!NOTE]
>
>您可以使用Workfront连接连接到Workfront展示板，也可以创建单独的Workfront展示板连接。

要创建Workfront展示板连接，请执行以下操作：

1. 在任何 [!DNL Adobe Workfront Boards] 模块，单击 **[!UICONTROL 添加]** ，位于“Connection（连接）”框旁。

1. 填写以下字段：

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[！UICONTROL连接名称]</td>
          <td>
            <p>输入此连接的名称。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL环境]</td>
          <td>选择您要连接到生产环境还是非生产环境。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL类型]</td>
          <td>选择您是要连接到服务帐户还是个人帐户。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL客户端ID]<p>（可选）</p></td>
          <td>输入您的 [!DNL Adobe] [！UICONTROL客户端ID]。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL客户端密钥]<p>（可选）</p></td>
          <td>输入您的 [!DNL Adobe] [！UICONTROL客户端密钥]。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL身份验证URL]<p>（可选）</p></td>
          <td>输入您的Workfront实例将用于对此连接进行身份验证的URL。 <p>默认值为 <code>https://oauth.my.workfront.com/integrations/oauth2</code>.</p>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL主机前缀]</td>
          <td>输入您的主机前缀。<p>默认值为 <code>origin-</code>.</p>
        </tr>
      </tbody>
    </table>
1. 单击 **[!UICONTROL 继续]** 以保存连接并返回到模块。

## Adobe Workfront展示板模块及其字段

配置Workfront展示板模块时， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些以外，还可能会显示其他Workfront展示板字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [信息卡](#cards)
* [展示板](#boards)
* [列](#columns)
* [标记](#tags)
* [其他](#other)

<!--

### Watch

#### Watch events

This trigger module starts a scenario when an event occurs on a board.

1. Click **[!UICONTROL Add]** to the right of the **Webhook** box.

1. Configure the webhook in the **[!UICONTROL Add a hook]** box that displays.

   When you are configuring this module, the following fields display.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>(Optional) Type a new name for the webhook</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>You can use an existing Workfront connection to connect to Workfront Boards, or you can use a specific Workfront Boards connection. </p><p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Create a connection to Workfront Boards</a> in this article.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Object type]</td> 
      <td>Select the type of [!DNL Workfront] object that you want the module to watch.</td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Objects to watch]</p> </td> 
      <td> Select whether you want to trigger a scenario when there is a new object, an updated object, a new or updated object, or a deleted object. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclude events made by this connection</td> 
      <td>Enable this option to exclude events created or updated using the same connector that this trigger module uses. This can prevent situations where a scenario might trigger itself, causing it to repeat in an endless loop.</td> 
     </tr> 
    </tbody> 
   </table>

After the webhook is created, you can view the address of the endpoint that events are sent to.

-->

### 信息卡

* [添加清单项目](#add-checklist-item)
* [添加子任务](#add-subtask)
* [创建信息卡](#create-a-card)
* [移动信息卡](#move-a-card)
* [读取信息卡](#read-a-card)
* [更新信息卡](#update-a-card)

#### 添加清单项目

此操作模块将一个清单项目添加到指定的信息卡。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用现有的Workfront连接连接到Workfront展示板，也可以使用特定的Workfront展示板连接。 </p><p>有关连接 [!DNL Workfront] 应用到 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">创建与Workfront展示板的连接</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL卡ID]</td> 
   <td>输入或映射您要将清单项目添加到的卡的ID。<p>在Workfront中查看信息卡时，您可以在URL中找到该信息卡ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL清单项目]</td> 
   <td>对于要添加的每个清单项目，单击“添加项目”，输入清单项目的名称，然后选择该项目是否已完成。</p></td> 
  </tr> 
 </tbody> 
</table>

#### 添加子任务

此操作模块将一个子任务添加到展示板中的信息卡。 该卡必须是已连接的卡。 该子任务也会添加到卡所代表的Workfront任务中。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用现有的Workfront连接连接到Workfront展示板，也可以使用特定的Workfront展示板连接。 </p><p>有关连接 [!DNL Workfront] 应用到 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">创建与Workfront展示板的连接</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL父卡片ID]</td> 
   <td>输入或映射要添加子任务的卡的ID。<p>在Workfront中查看信息卡时，您可以在URL中找到该信息卡ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>输入或映射包含要向其添加子任务的卡片的展示板的ID。<p>在Workfront中查看展示板时，您可以在URL中找到展示板ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL名称]</td> 
   <td>输入或映射新子任务的名称。</p></td> 
  </tr> 
 </tbody> 
</table>

#### 创建信息卡

此操作模块可在Workfront展示板上创建新信息卡。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用现有的Workfront连接连接到Workfront展示板，也可以使用特定的Workfront展示板连接。 </p><p>有关连接 [!DNL Workfront] 应用到 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">创建与Workfront展示板的连接</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>输入或映射要将信息卡添加到的展示板的ID。<p>在Workfront中查看展示板时，您可以在URL中找到展示板ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL列ID]</td> 
   <td>输入或映射要添加子任务的列的ID。<p>您可以从读取展示板模块返回的信息中找到标记ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL名称]</td> 
   <td>输入或映射新卡的名称。</p></td> 
  </tr> 
 </tbody> 
</table>

#### 移动信息卡

该操作模块可将一张信息卡移动到同一展示板上的另一列。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用现有的Workfront连接连接到Workfront展示板，也可以使用特定的Workfront展示板连接。 </p><p>有关连接 [!DNL Workfront] 应用到 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">创建与Workfront展示板的连接</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL卡ID]</td> 
   <td>输入或映射要移动的卡的ID。<p>在Workfront中查看信息卡时，您可以在URL中找到该信息卡ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>输入或映射包含要移动的信息卡的主板的ID。<p>在Workfront中查看信息卡时，您可以在URL中找到该信息卡ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目标列ID]</td> 
   <td>输入或映射要将卡片移动到的列的ID。<p>您可以从读取展示板模块返回的信息中找到标记ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL到索引]</td> 
   <td>输入或映射您希望信息卡在新列中的位置。<p>索引0中列的顶部位置。</p></td> 
  </tr> 
 </tbody> 
</table>

#### 读取信息卡

此操作模块可检索有关特定信息卡的信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用现有的Workfront连接连接到Workfront展示板，也可以使用特定的Workfront展示板连接。 </p><p>有关连接 [!DNL Workfront] 应用到 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">创建与Workfront展示板的连接</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL卡ID]</td> 
   <td>输入或映射要读取的信息卡的ID。<p>在Workfront中查看信息卡时，您可以在URL中找到该信息卡ID。</p></td> 
  </tr> 
 </tbody> 
</table>

#### 更新信息卡

此操作模块会更新您指定信息卡的信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用现有的Workfront连接连接到Workfront展示板，也可以使用特定的Workfront展示板连接。 </p><p>有关连接 [!DNL Workfront] 应用到 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">创建与Workfront展示板的连接</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL卡ID]</td> 
   <td>输入或映射要更新的信息卡的ID。<p>在Workfront中查看信息卡时，您可以在URL中找到该信息卡ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>输入或映射包含要更新的卡的主板的ID。<p>在Workfront中查看信息卡时，您可以在URL中找到该信息卡ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL名称]</td> 
   <td>输入或映射卡的新名称。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL卡ID]</td> 
   <td>输入或映射卡的新描述/\。</p></td> 
  </tr> 
 </tbody> 
</table>

### 展示板

* [创建展示板](#create-a-board)
* [阅读讨论区](#read-a-board)

#### 创建展示板

此操作模块可在Workfront中创建展示板。 您可以指定要创建的展示板类型。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用现有的Workfront连接连接到Workfront展示板，也可以使用特定的Workfront展示板连接。 </p><p>有关连接 [!DNL Workfront] 应用到 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">创建与Workfront展示板的连接</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板名称]</td> 
   <td>输入或映射新讨论区的名称。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL类型]</td> 
   <td>选择要创建的展示板类型。</td> 
  </tr> 
 </tbody> 
</table>

#### 阅读讨论区

此操作模块返回有关单个展示板的信息，例如展示板的卡片、列、标记和成员。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用现有的Workfront连接连接到Workfront展示板，也可以使用特定的Workfront展示板连接。 </p><p>有关连接 [!DNL Workfront] 应用到 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">创建与Workfront展示板的连接</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>输入或映射要检索其信息的展示板的ID。<p>在Workfront中查看展示板时，您可以在URL中找到展示板ID。</p></td> 
  </tr> 
 </tbody> 
</table>

### 列

#### 创建列

此操作模块在指定的展示板上创建新列。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用现有的Workfront连接连接到Workfront展示板，也可以使用特定的Workfront展示板连接。 </p><p>有关连接 [!DNL Workfront] 应用到 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">创建与Workfront展示板的连接</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>输入或映射要添加列的展示板的ID。<p>在Workfront中查看展示板时，您可以在URL中找到展示板ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL列名称]</td> 
   <td>输入或映射新列的名称。</td> 
  </tr> 
 </tbody> 
</table>

### 标记

* [向信息卡添加标记](#add-card-tag)
* [创建标记](#create-a-tag)

#### 向信息卡添加标记

此操作模块会将标记添加到信息卡。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用现有的Workfront连接连接到Workfront展示板，也可以使用特定的Workfront展示板连接。 </p><p>有关连接 [!DNL Workfront] 应用到 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">创建与Workfront展示板的连接</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL卡ID]</td> 
   <td>输入或映射要添加标记的卡的ID。<p>在Workfront中查看信息卡时，您可以在URL中找到该信息卡ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>输入或映射包含要将标记添加到的卡的展示板的ID。<p>在Workfront中查看展示板时，您可以在URL中找到展示板ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL标记ID]</td> 
   <td>输入或映射要添加标记的ID。<p>您可以从读取展示板模块返回的信息中找到标记ID。</p></td> 
  </tr> 
 </tbody> 
</table>

#### 创建标记

此操作模块将创建一个新标记并为其分配一种颜色。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用现有的Workfront连接连接到Workfront展示板，也可以使用特定的Workfront展示板连接。 </p><p>有关连接 [!DNL Workfront] 应用到 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">创建与Workfront展示板的连接</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>输入或映射要为其创建标记的展示板的ID。<p>在Workfront中查看展示板时，您可以在URL中找到展示板ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL标记名称]</td> 
   <td>输入或映射新标记的名称。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL标记颜色]</td> 
   <td>选择此标记的颜色。</td> 
  </tr> 
 </tbody> 
</table>

### 其他

#### 进行自定义API调用

此操作模块对Workfront展示板API进行自定义调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
      <td> <p>您可以使用现有的Workfront连接连接到Workfront展示板，也可以使用特定的Workfront展示板连接。 </p><p>有关连接 [!DNL Workfront] 应用到 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">创建与Workfront展示板的连接</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>输入相对路径<code> https://&lt;WORKFRONT_DOMAIN&gt;/boards-service/graphql?</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p><p>对于大多数展示板调用，方法POST。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。 这会确定请求的内容类型。</p> <p>例如，<code> { "Content-type":"application/json-stringify()"}</code></p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>对于Workfront展示板，此部分通常留空。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以JSON嵌入Graphql的形式添加API调用的正文内容 </p> <p>示例：</p><p>此示例更新列名。 您可以包含 <code>boardId</code> 和 <code>columnId</code> 作为GUID，硬编码或从以前的模块映射。<p><pre>{

  &quot;query&quot;： &quot;mutation { updateColumn(boardId： \&quot;\&quot;， columnId： \&quot;\&quot;， updateColumnInput： { name： \&quot;\&quot; }) { id name }}&quot;

}</pre><p>注意：  <p>使用条件语句(例如 <code>如果</code> 在JSON中，将引号放在条件语句之外。</p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p>
</div> </p> </td>
</tr> 
 </tbody> 
</table>
