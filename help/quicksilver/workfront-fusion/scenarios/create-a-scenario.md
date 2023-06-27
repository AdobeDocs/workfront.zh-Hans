---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在Adobe Workfront Fusion中创建方案
description: 以下任务说明如何创建 [!DNL Adobe Workfront Fusion] 场景。
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1422'
ht-degree: 0%

---

# 在中创建方案 [!DNL Adobe Workfront Fusion]

以下任务说明如何创建 [!DNL Adobe Workfront Fusion] 场景。

有关引导您创建自动化场景的练习练习，请参阅 [在中创建实践自动化方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

有关指导您使用我们提供的数据创建集成场景的练习练习，请参阅 [在Adobe Workfront Fusion中创建实践集成场景](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>要从模板创建方案，请参阅 [创建方案 [!DNL Adobe Workfront Fusion] 模板](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

## 访问要求

您必须具有以下权限才能使用本文中的功能：

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
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td> <p>[！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p><p>[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p><p>[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 开始创建方案

1. 单击 **[!UICONTROL 方案]** ![](assets/scenarios-icon.png) （在左侧面板中）。

1. 单击 **[!UICONTROL 创建新方案]** 页面右上角的。
1. 在显示的屏幕（方案编辑器）中，如果您要创建新方案，请单击 **[!UICONTROL 新方案]** 并键入方案的名称。
1. 继续到 [在场景中添加模块](#add-a-module-in-a-scenario).

## 在场景中添加模块

1. 要将第一个模块添加到方案，请单击问号图标。 ![](assets/question-mark-icon.gif)

   或

   要向场景中添加其他模块，请单击您希望场景遵循的模块右侧的句柄。

1. 在显示的框中，查找并单击要开始使用的应用程序或服务。

   之前选择的任何应用程序都会显示在框中，以便轻松访问，并且会显示在 **[!UICONTROL 收藏夹]** 部分（位于屏幕底部）。

   如果您单击 **[!UICONTROL 添加另一个模块]**，显示的模块取决于您在场景中添加模块的位置。 某些模块只能放在其他模块之间，而其他模块只能放在场景的开头处。

   >[!TIP]
   >
   >最常见的两类模块是操作和触发器。 有关更多信息，请参阅 [模块类型](../../workfront-fusion/modules/module-types.md).

1. 在显示的模块列表中，单击要添加到方案中的第一个模块。

   显示的模块取决于要在场景中添加模块的位置。 某些模块只能放在其他模块之间，而其他模块只能放在场景的开头处。

   最常见的两类模块是操作和触发器。 有关更多信息，请参阅 [模块类型](../../workfront-fusion/modules/module-types.md).

1. 继续到 [将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## 将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

连接到应用程序的Workfront Fusion模块(例如 [!DNL Workfront]， [!DNL Salesforce]，或 [!DNL Jira)] 特性 [!UICONTROL 连接] 字段。 在这里，您可以指定希望此模块用于连接到应用程序的连接。 您可以从下拉菜单中选择现有连接，也可以创建新连接。

当您为场景中的应用程序选择或创建连接时，该应用程序的其他模块会自动使用相同的连接，除非您在设置后面的模块时选择其他模块。

有关更多信息，请参阅 [关于连接 [!DNL Adobe Workfront Fusion] 至应用程序或服务](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

在内部创建连接 [!DNL Workfront Fusion] 模块：

1. 单击 **[!UICONTROL 添加]** 以打开 **[!UICONTROL 创建连接]** 盒子。
1. （可选）更改默认值 **[!UICONTROL 连接名称]**.
1. （视情况而定）如果应用程序需要高级连接设置，例如ID、键或 [!UICONTROL 密码]，请输入该信息。

   您可能需要单击 **[!UICONTROL 显示高级设置]** 以显示可在其中输入此类信息的字段。

1. 单击 **[!UICONTROL 继续]**.
1. 在显示的登录窗口中，输入您的凭据以登录到应用程序（如果尚未登录）。
1. （视情况而定）如果 **[!UICONTROL 允许]** 按钮显示，检查连接器能够执行的操作，然后单击按钮以将应用程序连接到 [!DNL Workfront Fusion].
1. 继续到 [配置模块](#configure-the-module).


## 配置模块

1. 在“连接”字段下面的字段中，配置模块的设置，然后单击 **[!UICONTROL 确定]**.

   ![](assets/conf-settigs-mod-350x547.png)

   每个模块的这些设置各不相同。 粗体标题表示所需的设置。

   >[!TIP]
   >
   >在处理场景时，您可以随时单击模块以显示此设置框。
   >
   >
   >如果在模块上看到一个黑色圆圈，则表示尚未完成其设置的配置。 单击模块以将其打开并继续配置。
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. 如果要向方案中添加第一个模块，请选择一个选项以指示每次运行方案时希望方案的启动位置。

   ![](assets/choose-where-start-350x194.png)

1. 重复各节中的步骤 [在场景中添加模块](#add-a-module-in-a-scenario) 和 [配置模块](#configure-the-module) 以向场景中添加其他模块。

1. （可选）复制并粘贴一个模块或模块组。

   有关更多信息，请参阅 [复制Adobe Workfront Fusion中的模块或场景](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. 继续到 [配置和使用场景](#configure-and-work-with-your-scenario).

## 配置和使用场景

1. 执行以下任一操作以配置方案：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">指定场景执行的时间和频率</td> 
      <td> <p>单击时钟图标。 </p> <p> <img src="assets/clock-icon.gif"> </p> <p>有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">在中计划方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">设置工艺路线</td> 
      <td> <p>单击扳手图标 <img src="assets/wrench-icon.gif"> ，并使用以下任一选项。 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">将过滤器添加到中的方案 [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[！UICONTROL设置过滤器]</strong>：控制场景中的某些时间点使用的包。</li> 
        <li><strong>[！UICONTROL取消链接]</strong>：删除路由。</li> 
        <li><strong>[！UICONTROL添加路由器]</strong>：在模块之间添加路由器。 </li> 
        <li><strong>[！UICONTROL添加模块]</strong>：在模块之间添加新模块。</li> 
        <li><strong>[！UICONTROL添加注释]</strong>：向路由添加注释。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">配置方案设置</td> 
      <td>单击[！UICONTROL方案设置]图标。 <img src="assets/gear-icon-settings.png"> 这些设置主要面向高级用户。 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">中的方案设置面板 [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">配置流量控制设置</td> 
      <td> <p>单击[！UICONTROL流量控制]图标。 <img src="assets/flow-control-icon.gif"> 您可以将任务设置为重复给定的次数，将数组转换为一系列捆绑包，然后将多个捆绑包合并为一个捆绑包。 有关更多信息，请参阅 <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">中的流量控制 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">使用高级工具增强场景</td> 
      <td>单击 [!DNL Tools] 图标。 <img src="assets/tools-icon.gif"> 您可以创建触发器、操作、聚合器和转换器。 有关更多信息，请参阅 <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">工具</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">用户文本解析工具</td> 
      <td>单击 [!DNL Text parser] 图标 <img src="assets/text-parser-icon.gif">. 您可以从HTML代码中检索元素、查找和提取与搜索模式匹配的字符串元素、搜索和替换文本，以及从网站中“擦除”数据。 有关更多信息，请参阅 <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">工具</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 执行以下任一操作以使用您的方案：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">查看场景运行时发生的事件日志</td> 
      <td> <p>单击[！UICONTROL退出编辑]箭头 <img src="assets/exit-editing-arrow.png"> 在方案编辑器中查看方案详细信息页面。 日志显示在窗口底部或右下角。 它包含有关每个阶段的信息以及在执行场景期间遇到的任何错误。</p> <p>要返回到“ ”中使用场景，请执行以下操作 [!DNL scenario editor]，单击“方案详细信息”页面上的任意位置。</p> <p>有关“方案详细信息”页面的详细信息，请参见 <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">中的方案详细信息 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">访问您最常用的应用程序和服务</td> 
      <td> 单击 <strong>[！UICONTROL收藏夹]</strong> 部分（位于屏幕底部）。 向方案添加应用程序和服务时，此部分会自动显示图标。 您还可以单击[！UICONTROL Add]图标 <img src="assets/add-icon.gif"> 以手动将应用和服务添加到此区域。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">查看显示数据如何流经场景的动画</td> 
      <td>单击[！UICONTROL解释流]图标 <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自动对齐模块的布局 </td> 
      <td>单击[！UICONTROL自动对齐]图标 <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">键入或查看有关方案的注释</td> 
      <td>单击[！UICONTROL注释]图标 <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除模块</td> 
      <td>右键单击模块，然后单击 <strong>[！UICONTROL删除模块]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 要测试运行方案，请单击 **[!UICONTROL 运行一次]**.

   在激活场景之前，务必验证场景是否可按预期运行。 一旦激活，场景将根据其计划执行。 如果所有内容都未按预期运行，请参见 [中的错误处理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. 完成方案编辑后（或在编辑过程中任何时间），单击 [!UICONTROL 保存] 图标（窗口底部） ![](assets/save-icon.gif).

有关激活场景的信息，请参阅 [在中激活或取消激活方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Workfront Fusion场景键盘快捷键

创建或编辑场景时，可以使用以下键盘快捷键：

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
   <td role="rowheader">[！UICONTROL保存] </td> 
   <td>Ctrl+Shift+S</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL运行一次]</td> 
   <td>Ctrl+Shift+Enter</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+Enter</span> </td> 
  </tr> 
 </tbody> 
</table>
