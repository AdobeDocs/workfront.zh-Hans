---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在Adobe Workfront Fusion中创建方案
description: 以下任务说明如何创建 [!DNL Adobe Workfront Fusion] 情景。
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '1428'
ht-degree: 0%

---

# 在中创建方案 [!DNL Adobe Workfront Fusion]

以下任务说明如何创建 [!DNL Adobe Workfront Fusion] 情景。

有关指导您创建自动化方案的实践练习，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

有关指导您使用我们提供的数据创建集成方案的实践练习，请参阅 [在Adobe Workfront Fusion中创建实践集成方案](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>要从模板创建方案，请参阅 [创建方案 [!DNL Adobe Workfront Fusion] 模板](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p>    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 开始创建方案

1. 单击 **[!UICONTROL 方案]** ![](assets/scenarios-icon.png) 中。

1. 单击 **[!UICONTROL 创建新方案]** 的双曲余切值。
1. （可选）在 **[!UICONTROL 您希望集成哪些服务]**，如果要创建新方案，请选择要在该方案中使用的应用程序，然后单击 **[!UICONTROL 继续]**.

   或

   单击 **[!UICONTROL 跳过]** 要从方案编辑器中选择应用程序时，请执行以下操作：

1. 在显示的屏幕（方案编辑器）中，如果要创建新方案，请单击 **[!UICONTROL 新方案]** 并键入方案的名称。
1. 继续 [在方案中添加模块](#add-a-module-in-a-scenario).

## 在方案中添加模块

1. 要将第一个模块添加到方案中，请单击问号图标。 ![](assets/question-mark-icon.gif)

   或

   要向方案中添加其他模块，请单击要跟踪的模块右侧的句柄。

1. 在显示的框中，找到并单击要开始使用的应用程序或服务。

   之前选择的任何应用程序都会显示在框中以供轻松访问，并且位于 **[!UICONTROL 收藏夹]** 的位置。

   如果单击 **[!UICONTROL 添加其他模块]**，显示的模块取决于您在场景中添加模块的位置。 某些模块只能放置在其他模块之间，而其他模块只能放置在方案开始时。

   >[!TIP]
   >
   >最常见的两种模块类型是操作和触发器。 有关更多信息，请参阅 [模块类型](../../workfront-fusion/modules/module-types.md).

1. 在显示的模块列表中，单击要添加到方案中的第一个模块。

   显示的模块取决于您希望在方案中添加模块的位置。 某些模块只能放置在其他模块之间，而其他模块只能放置在方案开始时。

   最常见的两种模块类型是操作和触发器。 有关更多信息，请参阅 [模块类型](../../workfront-fusion/modules/module-types.md).

1. 继续 [将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## 将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

Workfront Fusion模块，用于连接到应用程序(例如 [!DNL Workfront], [!DNL Salesforce]或 [!DNL Jira)] 功能 [!UICONTROL 连接] 字段。 在此，您可以指定您希望此模块用于连接到应用程序的连接。 您可以从下拉菜单中选择现有连接，或创建新连接。

当您在方案中为某个应用程序选择或创建连接时，该应用程序的其他模块会自动使用相同的连接，除非您在设置后续模块时选择其他连接。

有关更多信息，请参阅 [关于连接 [!DNL Adobe Workfront Fusion] 到应用程序或服务](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

在 [!DNL Workfront Fusion] 模块：

1. 单击 **[!UICONTROL 添加]** 打开 **[!UICONTROL 创建连接]** 框中。
1. （可选）更改默认 **[!UICONTROL 连接名称]**.
1. （视情况而定）如果应用程序需要高级连接设置，例如ID、键或 [!UICONTROL 秘密]，输入该信息。

   您可能需要单击 **[!UICONTROL 显示高级设置]** 以显示可在其中输入此类信息的字段。

1. 单击 **[!UICONTROL 继续]**.
1. 在显示的登录窗口中，输入您的凭据以登录到应用程序（如果尚未登录）。
1. （视情况而定）如果 **[!UICONTROL 允许]** 按钮，检查连接器能够执行的操作，然后单击按钮以将应用程序连接到 [!DNL Workfront Fusion].
1. 继续 [配置模块](#configure-the-module).


## 配置模块

1. 在“连接”字段下方的字段中，配置模块的设置，然后单击 **[!UICONTROL 确定]**.

   ![](assets/conf-settigs-mod-350x547.png)

   每个模块的这些设置各不相同。 标题为粗体表示必需的设置。

   >[!TIP]
   >
   >在您处理方案时，您可以随时单击模块以显示此设置框。
   >
   >
   >如果在模块上看到一个黑色圆圈，则表示尚未完成其设置的配置。 单击模块以将其打开并继续配置。
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. 如果要在方案中添加第一个模块，请选择一个选项以指示您希望方案每次运行时从何处开始。

   ![](assets/choose-where-start-350x194.png)

1. 重复各节中的步骤 [在方案中添加模块](#add-a-module-in-a-scenario) 和 [配置模块](#configure-the-module) 向方案中添加其他模块。

1. （可选）复制并粘贴一个模块或一组模块。

   有关更多信息，请参阅 [复制Adobe Workfront Fusion中的模块或方案](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. 继续 [配置并使用您的方案](#configure-and-work-with-your-scenario).

## 配置并使用您的方案

1. 执行以下任一操作以配置方案：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">指定执行方案的时间和频率</td> 
      <td> <p>单击时钟图标。 </p> <p> <img src="assets/clock-icon.gif"> </p> <p>有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">在中计划方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">设置路由</td> 
      <td> <p>单击扳手图标 <img src="assets/wrench-icon.gif"> 使用以下任意选项。 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">在 [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[!UICONTROL设置过滤器]</strong>:控制在场景中的特定点使用哪些包。</li> 
        <li><strong>[!UICONTROL取消链接]</strong>:删除路由。</li> 
        <li><strong>[!UICONTROL添加路由器]</strong>:在模块之间添加路由器。 </li> 
        <li><strong>[!UICONTROL添加模块]</strong>:在模块之间添加新模块。</li> 
        <li><strong>[!UICONTROL添加注释]</strong>:向路由添加注释。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">配置方案设置</td> 
      <td>单击[!UICONTROL方案设置]图标。 <img src="assets/gear-icon-settings.png"> 这些设置主要面向高级用户。 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">中的“方案设置”面板 [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">配置流量控制设置</td> 
      <td> <p>单击[!UICONTROL Flow Control]图标。 <img src="assets/flow-control-icon.gif"> 您可以设置任务以重复指定次数，将数组转换为一系列包，然后将多个包合并到一个包中。 有关更多信息，请参阅 <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">中的流量控制 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">使用高级工具增强方案</td> 
      <td>单击 [!DNL Tools] 图标。 <img src="assets/tools-icon.gif"> 您可以创建触发器、操作、聚合器和变压器。 有关更多信息，请参阅 <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">工具</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">用户文本解析工具</td> 
      <td>单击 [!DNL Text parser] 图标 <img src="assets/text-parser-icon.gif">. 您可以从HTML代码中检索元素，查找和提取与搜索模式匹配的字符串元素，搜索和替换文本，以及从网站中“抓取”数据。 有关更多信息，请参阅 <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">工具</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 执行以下任一操作以处理您的方案：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">查看运行方案时发生的事件的日志</td> 
      <td> <p>单击[!UICONTROL退出编辑]箭头 <img src="assets/exit-editing-arrow.png"> 在方案编辑器中，查看方案详细信息页面。 日志显示在窗口底部或右下角。 它包含有关每个阶段以及执行方案期间遇到的任何错误的信息。</p> <p>要在 [!DNL scenario editor]，单击“方案”详细信息页面上的任意位置。</p> <p>有关“方案”详细信息页面的更多信息，请参阅 <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">中的方案详细信息 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">访问最常用的应用程序和服务</td> 
      <td> 单击 <strong>[!UICONTROL收藏夹]</strong> 的位置。 当您向方案添加应用程序和服务时，此部分中会自动显示图标。 您还可以单击[!UICONTROL Add]图标 <img src="assets/add-icon.gif"> 手动将应用程序和服务添加到此区域。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">查看显示数据如何在场景中流动的动画</td> 
      <td>单击[!UICONTROL解释流程]图标 <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自动对齐模块的布局 </td> 
      <td>单击[!UICONTROL自动对齐]图标 <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">键入或查看有关方案的注释</td> 
      <td>单击[!UICONTROL Notes]图标 <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除模块</td> 
      <td>右键单击模块，然后单击 <strong>[!UICONTROL删除模块]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 要测试运行方案，请单击 **[!UICONTROL 运行一次]**.

   在激活方案之前，务必要验证方案是否按预期运行。 激活后，方案将根据其计划执行。 如果所有内容未按预期运行，请参阅 [在中处理错误 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. 编辑完方案（或在编辑时随时）后，单击 [!UICONTROL 保存] 图标 ![](assets/save-icon.gif).

有关激活方案的信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Workfront Fusion方案键盘快捷键

在创建或编辑方案时，您可以使用以下键盘快捷键：

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p>操作</p> </th> 
   <th>[!DNL Windows]</th> 
   <th> <p>[!DNL MacOS]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Save] </td> 
   <td>Ctrl+Shift+S</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL运行一次]</td> 
   <td>Ctrl+Shift+Enter</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+Enter</span> </td> 
  </tr> 
 </tbody> 
</table>
