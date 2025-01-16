---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 在 [!DNL Adobe Workfront Fusion]中创建实践自动化方案
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中创建实践自动化方案

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [用于创建方案的工作流](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/create-a-scenario-workflow.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

自动化场景可自动执行Workfront流程，包括数据操作和转换。 本文将引导您完成创建方案的过程，该方案将搜索项目，然后返回与该项目关联的所有任务。

<!-- not sure why these are here?
For instructions on building an integration scenario that connects separate apps, see [Create a practice integration scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

For more information on functionality available with each Workfront Fusion license, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

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

## 创建自动化实践方案

[!DNL Adobe Workfront Fusion]通过自动执行重复任务，帮助您专注于重要任务。 它创建场景以自动管理各种应用程序和服务中的数据。

每个方案都包含模块，用于指导如何在应用程序内处理数据或在不同的应用程序和服务之间传输数据。 例如，您可以在Fusion中创建方案以自动查找[!DNL Workfront]项目并列出其任务。 这样，Fusion就可以处理日常任务，从而为您节省时间和精力。

此实践方案将引导您完成创建方案的过程，该方案将搜索[!DNL Workfront]项目并返回项目中的任务。

![](assets/create-practice-scenario-wf-only-350x157.png)

### 开始之前

在Workfront中创建一个包含可用于本练习的任务的项目。 除了将任务添加到项目外，您无需执行任何其他配置。

有关在Workfront中创建项目的信息，请参见xxx。

### 1.创建方案并为其命名

1. 登录您的[!DNL Workfront Fusion]帐户。
1. 单击左侧面板中的&#x200B;**[!UICONTROL 方案]** ![](assets/scenarios-icon.png)。

   >[!NOTE]
   >
   >如果未看到左侧导航面板或其图标，请单击菜单![菜单](assets/main-menu-icon-left-nav.png)图标。

1. 在&#x200B;[!UICONTROL **文件夹**]&#x200B;面板中，单击&#x200B;**[!UICONTROL 添加文件夹]**&#x200B;图标![](assets/add-folder-icon.png)，然后为第一个文件夹键入诸如“实践场景”之类的名称。

1. 打开文件夹，然后单击页面右上角的&#x200B;**[!UICONTROL 创建新方案]**。

1. 对于此练习，请选择&#x200B;**[!DNL Adobe Workfront]**&#x200B;应用，然后单击底部附近的&#x200B;**搜索**。


1. 选择左上角的&#x200B;**[!UICONTROL 新方案]**&#x200B;占位符名称，然后键入诸如“实践方案1”之类的名称。

   ![](assets/name-the-scenario.png)

1. 继续[连接下面的第一个模块](#2-connect-the-first-module)。

### 2.连接第一个模块

现在，您需要与您的[!DNL Workfront]帐户建立经过身份验证的连接。 您添加到方案的每个模块都必须与其应用程序建立连接。

1. 在&#x200B;**[!DNL Workfront]**&#x200B;框的&#x200B;**[!UICONTROL 连接]**&#x200B;下，单击&#x200B;**[!UICONTROL 添加]**，然后键入连接的名称，如“Olivia的Workfront帐户”，然后单击&#x200B;**[!UICONTROL 继续]**。
1. 在显示的窗口中验证连接。

   对连接进行身份验证的过程在应用程序之间可能会有所不同。 以下进程特定于[!DNL Workfront]，但该进程与许多应用程序类似：

   1. 输入您的[!DNL Workfront]域，然后单击&#x200B;**[!UICONTROL 继续]**。
   1. 登录[!DNL Workfront]。
   1. 检查[!DNL Workfront Fusion]请求的访问，然后单击&#x200B;**[!UICONTROL 允许访问]**。

   如果需要帮助，请参阅[连接概述](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md)。

### 3.配置第一个模块

将[!DNL Workfront Fusion]连接到您的[!DNL Workfront]帐户后，您可以指定您有权访问的[!DNL Workfront]项目以及您希望第一个模块处理的数据。

1. 在[!UICONTROL 记录类型]框中，选择&#x200B;**[!UICONTROL 项目]**。 这将模块设置为仅搜索项目。

   >[!TIP]
   >
   >如果您开始输入“[!UICONTROL 项目]”，则可以在列表中找到&#x200B;**[!UICONTROL 项目]**。

1. 在&#x200B;**[!UICONTROL 结果集]**&#x200B;框中，选择&#x200B;**[!UICONTROL 第一个匹配记录]**。 这会将模块设置为仅返回它发现满足条件的第一个记录。 在本例中，我们只需要返回一个记录。
1. 在&#x200B;**[!UICONTROL 搜索条件]**&#x200B;区域，我们将设置过滤器以返回特定项目：

   | 字段 | 操作 |
   |--------|-------------|
   | 搜索条件字段 | 选择要搜索其值的字段。 对于此示例，请选择&#x200B;**[!UICONTROL 名称]**。 |
   | 搜索条件 | 在第一个下拉菜单中，选择&#x200B;**[!UICONTROL 名称]**。 |
   | 基本运算符 | 在第二个下拉菜单中，选择[!UICONTROL 包含（不区分大小写）]。 这允许模块查找名称中包含您选定字词的项目，即使您未输入完整名称或输入大小写不正确（例如全部大写）的名称，也是如此。 |
   | 文本框 | 输入您知道位于要搜索的项目名称中的单词或短语。 |

+++ 展开以查看屏幕上的示例。
   ![](assets/search-name.png)
+++

1. 在&#x200B;**[!UICONTROL 输出]**&#x200B;列表中，选择要模块输出的字段。 对于此示例，请选择&#x200B;**[!UICONTROL ID]**&#x200B;和&#x200B;**[!UICONTROL Name]**&#x200B;字段。

   >[!TIP]
   >
   >您可以使用&#x200B;**Cmd+F** （[!DNL Mac]操作系统）或&#x200B;**Ctrl-F** （[!DNL Windows]操作系统）快速查找字段。

1. 单击&#x200B;**[!UICONTROL 确定]**。

   >[!NOTE]
   >
   >由于这不是触发器模块，因此您不会选择从何处启动它。 使用触发器模块时，您现在可以选择从何处启动它。
   >
   >
   >有关详细信息，请参阅[选择触发器模块在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md)中的开始位置。

1. 右键单击该模块，单击“**[!UICONTROL 重命名]**”，键入描述您希望该模块执行的操作的名称（如“搜索项目”），然后单击“**[!UICONTROL 确定]**”。

   该名称显示在模块正下方。 在其下方，[!DNL Workfront Fusion]包含模块执行的操作类型的简要说明。

   ![](assets/module-renamed-wf.png)

1. 继续[添加并配置第二个模块](#add-and-configure-the-second-module)。

### 4.添加并配置第二个模块

1. 单击模块右侧的部分圆圈以&#x200B;**[!UICONTROL 添加另一个模块]**。
1. 从应用程序列表中选择[!DNL Workfront]，然后选择搜索模块&#x200B;**[!UICONTROL 读取相关记录]**。
1. 在&#x200B;**[!UICONTROL 连接]**&#x200B;框中，选择您为上一个模块创建的连接。 您必须确保此模块使用的连接与上一个模块相同。
1. 单击&#x200B;**[!UICONTROL 记录类型]**，然后选择&#x200B;**[!UICONTROL 项目]**，因为我们要读取与项目相关的记录。

   >[!TIP]
   >
   >如果您开始输入“项目”，则可以在列表中找到&#x200B;**[!UICONTROL 项目]**。

1. 单击&#x200B;**[!UICONTROL 父记录ID]**&#x200B;字段。 此字段要求您想要从中返回任务的项目的Workfront ID。

   单击该字段将打开可在&#x200B;**[!UICONTROL 父记录ID]**&#x200B;字段中使用的变量列表，以标识Workfront中的项目。

   ![](assets/list-of-available-variables-wf-350x368.png)

1. 单击变量&#x200B;**[!UICONTROL ID]**&#x200B;以将其添加到&#x200B;**[!UICONTROL 父记录ID]**&#x200B;字段。 这允许将从第一个模块返回的ID用作要在第二个模块中处理的项目的标识符，从而确保返回的任务将属于该项目。
1. 在&#x200B;**[!UICONTROL 收藏集]**&#x200B;字段中，选择&#x200B;**[!UICONTROL 任务]**。 这表示模块将返回与所选项目关联的任务。
1. 在&#x200B;**[!UICONTROL 输出]**&#x200B;字段中，选择&#x200B;**[!UICONTROL Id]**&#x200B;和&#x200B;**[!UICONTROL Name]**。
1. 单击&#x200B;**[!UICONTROL 确定]**

   现在您有一个可行的方案。

1. 为第二个模块命名，例如“返回与项目关联的任务”，然后继续[测试方案](#test-the-scenario)。

## 测试场景

在激活方案之前，请务必至少运行一次方案并查看结果以对其进行测试。 这有助于您了解数据如何在场景中流动并查找任何错误。

我们选择返回1个项目，以及与该项目关联的任务。 如果您运行场景，则应该发生这种情况。

1. 在方案编辑器的左下角单击&#x200B;**[!UICONTROL 运行一次]**。
1. 方案运行完毕后，单击第一个模块上方的气泡。

   ![](assets/click-bubble.png)

   在显示的框中，您可以查看有关模块处理的数据包的信息，包括从模块返回的项目中提取的实际数据。

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. 单击第二个模块上方的执行检查器气泡，可查看信息输入和输出，它是项目中包含的任务集合。

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   您可在以下文章中了解有关如何读取场景执行信息的更多信息：

   * 有关一般信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md)中的[方案执行流程。
   * 有关已处理捆绑包的信息，请参阅[方案执行、周期和 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)中的阶段。

1. 在[!DNL Workfront Fusion]中，单击左下角附近的&#x200B;**[!UICONTROL 保存]** ![](assets/save-icon.png)以保存方案进度。

   >[!IMPORTANT]
   >
   >在磨练和测试场景时经常保存。

>[!TIP]
>
>我们建议您选择添加有关每个模块的注释这一有用但可选的实践。
>
>1. 右键单击[!DNL Workfront]模块，然后单击&#x200B;**[!UICONTROL 添加备注]**。
>1. 在显示的注释中，键入模块的概述。
>
>    您可以为一个模块添加多个注释。
>
>1. 关闭&#x200B;**[!UICONTROL 注释]**&#x200B;区域。
>
>     向方案添加注释后，方案编辑器底部的&#x200B;**[!UICONTROL 注释]**&#x200B;图标![](assets/notes-icon-w-dot.png)上会显示一个橙色点。
>
>1. 单击&#x200B;**[!UICONTROL 备注]**&#x200B;图标![](assets/notes-icon-w-dot.png)查看您的备注。
>

## 激活方案

此示例方案没有触发器模块。 如果您将这种情况用于实际数据，则它将以触发模块开头，您的最后一个操作是激活它。 在激活方案后，默认情况下，它每15分钟运行一次。 您可以通过定义运行的时间和频率来更改此设置。

有关激活方案的详细信息，请参阅[在[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md)中激活或停用方案。

有关计划的信息，请参阅[在[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md)中计划方案。
