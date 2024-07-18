---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在Adobe Workfront Fusion中创建方案
description: 以下任务说明如何创建 [!DNL Adobe Workfront Fusion] 方案。
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: ee2283ac159ca26ca473cac28ec4bed85d1dea04
workflow-type: tm+mt
source-wordcount: '1406'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中创建方案

以下任务说明如何创建[!DNL Adobe Workfront Fusion]方案。

有关指导您创建自动化方案的练习练习，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)中创建自动化方案练习。

有关指导您使用我们提供的数据创建集成方案的实践练习，请参阅[在Adobe Workfront Fusion中创建实践集成方案](../../workfront-fusion/get-started/create-a-practice-scenario.md)。

>[!NOTE]
>
>要从模板创建方案，请参阅[使用 [!DNL Adobe Workfront Fusion] 模板创建方案](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront计划</td>  
      <td>任何</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront许可证</td>  
      <td>
        新建： Standard<br>
        或<br>
        当前：工作或更高
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion许可证</td>  
      <td> 
        当前：无Workfront Fusion许可证要求。<br>
        或<br>
        旧版：任意
      </td>  
    </tr>  
    <tr>  
      <td>产品</td>  
      <td> 
        新文档：选择或Prime Workfront计划：您的组织必须购买Adobe Workfront Fusion。<br>
        Ultimate Workfront计划：包含Workfront Fusion。<br>
        或<br>
        当前：您的组织必须购买Adobe Workfront Fusion。
      </td>  
    </tr> 
  </tbody>  
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

+++

## 开始创建方案

1. 单击左侧面板中的&#x200B;**[!UICONTROL 方案]** ![](assets/scenarios-icon.png)。

1. 单击页面右上角的&#x200B;**[!UICONTROL 创建新方案]**。
1. 在显示的屏幕（方案编辑器）中，如果要创建新方案，请单击左上角的&#x200B;**[!UICONTROL 新建方案]**，然后键入方案的名称。
1. 继续[在方案](#add-a-module-in-a-scenario)中添加模块。

## 在场景中添加模块

1. 要将第一个模块添加到方案，请单击问号图标。![](assets/question-mark-icon.gif)

   或

   要向场景中添加其他模块，请单击您希望场景遵循的模块右侧的手柄。

1. 在显示的框中，查找并单击要开始使用的应用程序或服务。

   之前选择的任何应用都将显示在框内，以便于访问，并显示在屏幕底部的&#x200B;**[!UICONTROL 收藏夹]**&#x200B;部分中。

   如果单击“**[!UICONTROL 添加另一个模块]**”，则显示的模块取决于添加该模块的方案中所处的位置。 某些模块只能放置在其他模块之间，而其他模块只能放置在场景的开头处。

   >[!TIP]
   >
   >两种最常见的模块类型是操作和触发器。 有关详细信息，请参阅[模块类型](../../workfront-fusion/modules/module-types.md)。

1. 在显示的模块列表中，单击要添加到方案中的第一个模块。

   显示的模块取决于要在场景中添加模块的位置。 某些模块只能放置在其他模块之间，而其他模块只能放置在场景的开头处。

   两种最常见的模块类型是操作和触发器。 有关详细信息，请参阅[模块类型](../../workfront-fusion/modules/module-types.md)。

1. 继续[将模块的应用或Web服务连接到 [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion)。

## 将模块的应用或Web服务连接到[!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

连接到应用程序（如[!DNL Workfront]、[!DNL Salesforce]或[!DNL Jira)]）的Workfront Fusion模块具有[!UICONTROL 连接]字段。 在这里，您可以指定希望此模块用于连接到应用程序的连接。 您可以从下拉列表中选择现有连接，也可以创建新连接。

当您在场景中选择或创建应用程序的连接时，除非您在设置后续模块时选择其他连接，否则该应用程序的其他模块会自动使用相同的连接。

有关详细信息，请参阅[连接概述](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md)。

![](assets/connection-field-350x169.png)

要在[!DNL Workfront Fusion]模块内创建连接，请执行以下操作：

1. 单击&#x200B;**[!UICONTROL 添加]**&#x200B;打开&#x200B;**[!UICONTROL 创建连接]**&#x200B;框。
1. （可选）更改默认&#x200B;**[!UICONTROL 连接名称]**。
1. （有条件）如果应用程序需要高级连接设置（如ID、密钥或[!UICONTROL 密钥]），请输入该信息。

   您可能需要单击&#x200B;**[!UICONTROL 显示高级设置]**&#x200B;以显示可在其中输入此类信息的字段。

1. 单击&#x200B;**[!UICONTROL 继续]**。
1. 在显示的登录窗口中，输入您的凭据以登录应用程序（如果尚未登录）。
1. （视情况而定）如果显示&#x200B;**[!UICONTROL 允许]**&#x200B;按钮，请检查连接器能够执行的操作，然后单击按钮以将应用程序连接到[!DNL Workfront Fusion]。
1. 继续[配置模块](#configure-the-module)。


## 配置模块

1. 在“连接”字段下面的字段中，配置模块的设置，然后单击&#x200B;**[!UICONTROL 确定]**。

   ![](assets/conf-settigs-mod-350x547.png)

   每个模块的这些设置各不相同。 粗体标题表示所需的设置。

   >[!TIP]
   >
   >在处理方案时，您可以随时单击模块以显示此设置框。
   >
   >
   >如果在模块上看到黑色圆圈，则表示您尚未完成其设置的配置。 单击模块以将其打开并继续配置。
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. 如果要添加方案中的第一个模块，请选择一个选项，以指示每次运行方案时希望方案的启动位置。

   ![](assets/choose-where-start-350x194.png)

1. 重复[在场景中添加模块](#add-a-module-in-a-scenario)和[配置模块](#configure-the-module)中的步骤以向场景中添加其他模块。

1. （可选）复制并粘贴一个模块或模块组。

   有关详细信息，请参阅[复制Adobe Workfront Fusion中的模块或方案](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)。

1. 继续[配置和使用方案](#configure-and-work-with-your-scenario)。

## 配置和使用场景

1. 执行以下任一操作以配置方案：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">指定方案执行的时间和频率</td> 
      <td> <p>单击时钟图标。 </p> <p> <img src="assets/clock-icon.gif"> </p> <p>有关详细信息，请参阅<a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中计划方案。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">设置工艺路线</td> 
      <td> <p>单击两个模块之间的扳手图标<img src="assets/wrench-icon.gif">，并使用以下任一选项。 有关详细信息，请参阅<a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">将筛选器添加到[!DNL Adobe Workfront Fusion]</a>中的方案。</p> 
       <ul> 
        <li><strong>[！UICONTROL设置筛选器]</strong>：控制在场景中的某些点使用哪些包。</li> 
        <li><strong>[！UICONTROL Unlink]</strong>：删除路由。</li> 
        <li><strong>[！UICONTROL添加路由器]</strong>：在模块之间添加路由器。 </li> 
        <li><strong>[！UICONTROL添加模块]</strong>：在模块之间添加新模块。</li> 
        <li><strong>[！UICONTROL添加注释]</strong>：向路由添加注释。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">配置方案设置</td> 
      <td>单击[！UICONTROL方案设置]图标。 <img src="assets/gear-icon-settings.png">这些设置主要适用于高级用户。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">方案设置面板。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">配置流量控制设置</td> 
      <td> <p>单击[！UICONTROL流量控制]图标。 <img src="assets/flow-control-icon.gif">您可以将任务设置为重复给定次数，将数组转换为一系列捆绑包，并将多个捆绑包合并为一个捆绑包。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">流控制。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">使用高级工具增强场景</td> 
      <td>单击 [!DNL Tools] 图标。<img src="assets/tools-icon.gif">您可以创建触发器、操作、聚合器和转换器。 有关详细信息，请参阅<a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">工具</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">用户文本分析工具</td> 
      <td>单击[!DNL Text parser]图标<img src="assets/text-parser-icon.gif">。 您可以从HTML代码中检索元素、查找和提取与搜索模式匹配的字符串元素、搜索和替换文本，以及从网站“刮取”数据。 有关详细信息，请参阅<a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">工具</a>。</td> 
     </tr> 
    </tbody> 
   </table>

1. 可执行以下任一操作来处理您的场景：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">查看方案运行时发生的事件日志</td> 
      <td> <p>单击方案编辑器中的[！UICONTROL退出编辑]箭头<img src="assets/exit-editing-arrow.png">以查看方案详细信息页面。 日志显示在窗口底部或右下角。 它包含有关每个阶段的信息以及在执行场景期间遇到的任何错误。</p> <p>要重新在[!DNL scenario editor]中使用方案，请单击“方案详细信息”页面上的任意位置。</p> <p>有关“方案详细信息”页面的详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">方案详细信息。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">访问您最常用的应用程序和服务</td> 
      <td> 单击屏幕底部<strong>[！UICONTROL收藏夹]</strong>部分中的图标。 向方案添加应用和服务时，此部分会自动显示图标。 您还可以单击[！UICONTROL添加]图标<img src="assets/add-icon.gif">以手动将应用和服务添加到此区域。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">查看显示数据如何流经场景的动画</td> 
      <td>单击[！UICONTROL Explain flow]图标<img src="assets/explain-flow-airplane-icon.gif">。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自动对齐模块布局 </td> 
      <td>单击[！UICONTROL自动对齐]图标<img src="assets/auto-align-icon.gif">。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">键入或查看有关方案的说明</td> 
      <td>单击[！UICONTROL注释]图标<img src="assets/notes-icon.gif">。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除模块</td> 
      <td>右键单击模块，然后单击<strong>[！UICONTROL删除模块]</strong>。</td> 
     </tr> 
    </tbody> 
   </table>

1. 要测试运行方案，请单击&#x200B;**[!UICONTROL 运行一次]**。

   在激活场景之前，请验证场景是否按预期运行，这一点很重要。 一旦激活，场景将根据其计划执行。 如果所有组件都未按预期运行，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md)中的[错误处理。

1. 完成方案编辑后（或在编辑期间），单击窗口![](assets/save-icon.gif)底部的[!UICONTROL 保存]图标。

有关激活方案的信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md)中激活或停用方案。

## Workfront Fusion场景键盘快捷键

创建或编辑方案时，可以使用以下键盘快捷键：

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
