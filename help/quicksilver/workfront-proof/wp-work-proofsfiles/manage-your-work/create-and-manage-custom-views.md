---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 在中创建和管理自定义视图 [!DNL Workfront Proof]
description: 您可以创建文件和校样的自定义视图，以按您希望显示的方式列出所需项目。 您还可以将自定义视图中的信息导出为报表（以CSV格式，以逗号分隔值，文件格式）。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 7c6f3fdd-f767-4e8d-937a-1c7645aba55b
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '2457'
ht-degree: 1%

---

# 在中创建和管理自定义视图 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

您可以创建文件和校样的自定义视图，以按您希望显示的方式列出所需项目。 您还可以将自定义视图中的信息导出为报表（以CSV格式，以逗号分隔值，文件格式）。

>[!NOTE]
>
>自定义视图仅在“选择”和“高级”计划中可用。 请联系我们的销售团队获取报价。

## 创建自定义视图

创建自定义视图时，您可以选择：

* 是包含校样、文件，还是同时包含两者
* 显示哪些列
* 要排序的列
* 列的排序顺序（升序或降序）
* 用于确定视图中包含哪些信息的过滤器类型

创建自定义视图后，便可立即使用该视图。 新视图的名称也包含在标题“我的自定义视图”（位于“标准视图”下）下的下拉菜单中。

要创建自定义视图，请执行以下操作：

1. 转到 **[!UICONTROL 视图]** 页面。
1. 有关视图的更多信息，请参阅 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).
1. 根据您是要从头开始创建新的自定义视图，还是基于现有标准视图创建新的自定义视图，执行以下任一操作：

   * 要基于现有标准视图创建新的自定义视图，请执行以下操作：从下拉菜单中，选择要用作新自定义视图基础的现有标准视图。 单击 **[!UICONTROL 查看设置]** 图标，然后单击 **[!UICONTROL 复制]** 新建自定义视图。

   * ![](assets/proof-custom-view-icon.png)

   * 要从头开始创建新的自定义视图：单击 **[!UICONTROL 新建视图]** 图标。
   * ![](assets/proof-newview.png)

1. 在 **[!UICONTROL 详细信息]** ，请指定以下信息：

   * **[!UICONTROL 名称]** （必需）：新视图的名称。 使用唯一的名称，以便用户可以轻松地在“视图”的下拉菜单中找到自定义视图。
   * **[!UICONTROL 项目]**:选择是希望视图中同时包含校样和文件、仅校样，还是仅包含文件。 默认情况下，校样和文件都包含在内。

1. 在 **[!UICONTROL 列]** 部分，确定要在自定义视图中包含的列。

   1. 单击向右箭头图标。
   1. ![](assets/proof-view-rightarrow.png)

   1. 双击所选列的名称。
   1. 必须至少选择一个列，并且只能添加一列。
   1. 从 **[!UICONTROL 可用列]** 要包含在新视图中的区域。
   1. 列将从 **[!UICONTROL 可用列]** 列表 **[!UICONTROL 选定的列]** 列表。

   1. 您可以从标准列中进行选择，也可以选择自定义字段和决策原因作为自定义视图中的列。 （如果您在帐户中配置了这些列，则它们会显示在“可用列”区域的标准列表下。）
   1. 您可以包含的标准列

      <table style="table-layout:auto">
      <thead>

      </thead>
      <tbody>  
      <tr>   
      <td><strong>活动阶段名称</strong></td>   
      <td>自动化工作流中活动阶段的名称。</td>  
      </tr>  
      <tr>   
      <td><strong>注释</strong></td>   
      <td>收到的评论数。</td>
      </tr>  
      <tr>   
      <td><strong>计数器</strong></td>
      <td>显示已上载到您帐户的校样数量（您必须在帐户设置中启用校样计数器选项）。</td>
      </tr>
      <tr>
      <td><strong>已创建</strong></td>
      <td>创建项目的日期和时间。</td>
      </tr>
      <tr>
      <td><strong>创建者</strong></td>
      <td>创建项目的用户。</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL日期已添加到校样]</strong></td>
      <td>将您添加到校样的日期。 </td>
      </tr>
      <tr>
      <td><strong>截止日期</strong></td>
      <td>整个证明的截止日期。</td>
      </tr>
      <tr>
      <td><strong>决策</strong></td>
      <td>在预期数目中作出的决定的数目（如0/1、1/1等）</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL下载]</strong></td>
      <td>下载原始文件的次数。</td>
      </tr>
      <tr>
      <td><strong>文件名</strong></td>
      <td>文件或校样的名称。</td>
      </tr>
      <tr>
      <td><strong>文件夹</strong></td>
      <td>包含项目的文件夹。</td>
      </tr>
      <tr>
      <td><strong>上次活动</strong></td>
      <td>项目上最后一个活动的日期和时间。</td>
      </tr>
      <tr>
      <td><strong>最新决定</strong></td>
      <td>上次决策的日期和时间。</td>
      </tr>
      <tr>
      <td><strong>我的截止日期</strong></td>
      <td>您自己的校样截止日期，明确将您添加为审阅人/审批人（如果已应用）。</td>
      </tr>
      <tr>
      <td><strong>所有者</strong></td>
      <td>项目的所有者。</td>
      </tr>
      <tr>
      <td><strong>所有者国家/地区</strong></td>
      <td>系统中为证据所有者注册的国家/地区。 </td>
      </tr>
      <tr>
      <td><strong>父校样</strong></td>
      <td>父校样的名称。</td>
      </tr>
      <tr>
      <td><strong>进度</strong></td>
      <td><p>进度栏。 显示尚未开始、已打开、已评论或已决定的校样。</p><p>此信息未排序。</p></td>
      </tr>
      <tr>
      <td><strong>校对名称</strong></td>
      <td>校样的名称。</td>
      </tr>
      <tr>
      <td><strong>校样类型</strong></td>
      <td><p>校样类型：静态文件、静态网页、交互式Web（.zip上传）、交互式网页(https)、视频、音频和其他。 </p><p>组合校样被标识为“组合校样类型”。 校样的文件类型。</p></td>
      </tr>
      <tr>
      <td><strong>文件大小(MB)</strong></td>
      <td><p>校样的文件大小，与磁盘使用配额有关。</p><p>为当前版本的校样提供了此信息。 如果没有当前版本，则它适用于最新版本。</p></td>
      </tr>
      <tr>
      <td><p> </p><p><strong>活动阶段的截止时间</strong></p></td>
      <td>自动化工作流中各个阶段的截止日期。</td>
      </tr>
      <tr>
      <td><strong>阶段名称</strong></td>
      <td>自动工作流中每个阶段的名称。 这包括过去的阶段、活动的阶段和未来的阶段。</td>
      </tr>
      <tr>
      <td><strong>州/省</strong></td>
      <td>活动、锁定、草稿或已提交。</td>
      </tr>
      <tr>
      <td><strong>状态</strong></td>
      <td>待定、需要更改、已批准且已更改、已批准或不相关。</td>
      </tr>
      <tr>
      <td><strong>标记</strong></td>
      <td>附加到项目的任何标记。</td>
      </tr>
      <tr>
      <td><strong>即将推出的阶段名称</strong></td>
      <td> 自动化工作流中尚未启动的每个阶段的名称。 </td>
      </tr>
      <tr>
      <td><strong>版本计数器</strong></td>
      <td> 项目的版本数。 </td>
      </tr>
      <tr>
      <td><strong>校样版本号</strong></td>
      <td><i>校样的版本号。</i></td>
      </tr> 
      </tbody>
      </table>

   1. （可选）执行以下任一操作，将列移动到 **[!UICONTROL 选定的列]** 区域，以便将其包含在新视图中：

      * 对 **[!UICONTROL 选定的列]** 列表。
      * 列在 **[!UICONTROL 选定的列]** 列表确定列在自定义视图中的显示顺序。
      * 列在 **[!UICONTROL 选定的列]** 列表，其顺序为 **[!UICONTROL 可用列]** 列表。

      * 对 **[!UICONTROL 选定的列]** 列表中，选择列的名称，然后将其向上或向下拖动到列表中。

      * 从 **[!UICONTROL 选定的列]** 列表，单击选定列的名称，然后单击 **[!UICONTROL 左]** 箭头。 或者，您也可以双击所选列的名称(该列将移回 **[!UICONTROL 可用列]** 列表)。

      * 列只能添加一次。 例如，如果将“注释”列从 [!UICONTROL 可用] to [!UICONTROL 选定的列] 列表中，此列的名称将从 [!UICONTROL 可用列] 列表。

1. 在 **[!UICONTROL 排序]** ，请指定以下信息：

   * **排序依据：** 使用 [!UICONTROL 排序] 选项卡。 如果不选择要排序的列，则默认为“无”列 — 即，没有特殊排序列或顺序。
   * 仅在 [!UICONTROL 列] 选项卡 [!UICONTROL 按列排序] 下拉列表。
   * **升序或降序：** 选择是默认对列进行升序排序还是降序排序。

1. 使用 **[!UICONTROL 过滤器]** 定义一个或多个标准以选择要包含在“自定义”视图中的项目。 如果您希望将自定义视图用作报表，则过滤器会特别有用。
1. 要在自定义视图中包含所有项目，请跳过 **[!UICONTROL 过滤器]** 中。
1. 可用过滤器：

   * **字段：** 选择此过滤器的字段（默认字段为“注释”。） 字段列表包含所有标准字段(如 [!UICONTROL 列] 选项卡。 列表不限于您选择显示的列。
   * **运算符：** 过滤器可用的运算符取决于您选择的字段类型。 选择一个运算符，以显示字段与值字段之间的关系。 您稍后会填写此信息。
   * **值：** 根据您选择的字段和运算符，在此字段中选择或输入您选择的值。 根据您选择的运算符，可能有一个Value字段或两个或无。 请参阅以下示例。
   * **使用以下逻辑应用过滤器：** 不同字段之间的筛选条件将使用AND运算符。 使用同一字段的多个筛选条件将对同一字段使用OR运算符。

      如果只想查看具有零注释的校样，请选择以下值：

      * 字段：评论
      * 运算符：等于
      * 值字段：0

      如果只想查看包含两个或更多注释的校样，请选择以下值：

      * 字段：评论
      * 运算符：大于或等于
      * 值字段：2

      如果只想查看包含1到4条注释的校样，请选择以下值：

      * 字段：评论
      * 运算符：介于
      * 值字段（第一个字段）：1
      * 值字段（第二个字段）：4

         您可以更改已添加到自定义视图的过滤器，使其不出现任何问题，或通过单击 [!UICONTROL 设置] 过滤。

         因为字段列表不限于您在 [!UICONTROL 列] 选项卡，请注意在创建过滤器时，该过滤器中包含的列未选择在自定义视图中显示。 例如，以下视图筛选器将选择版本计数器值为2或更大的所有校样：

         * 字段=版本计数器
         * 运算符=大于或等于
         * 值字段= 2

            >[!NOTE]
            >
            >您可以更改已添加到自定义视图的过滤器，使其不出现任何问题，或通过单击 [!UICONTROL 设置] 过滤。





1. 在 **[!UICONTROL 共享]** 部分，选择您帐户中能够查看自定义视图的用户。
1. 自定义视图是特定于创建这些视图的用户。 默认情况下，新的“自定义”视图仅对其创建者可见；但是，您可以选择通过选择以下选项之一来共享自定义视图：

   * **只有您才能看到此自定义视图** （默认）：如果希望自定义视图仅供您使用，请选择此选项。
   * **所有用户都可以查看此自定义视图**:选择此选项可使自定义视图对您帐户上的所有用户可用。
   * **选择可以查看此自定义视图的用户**:选择此选项可使自定义视图仅对特定用户可用。
   * 开始键入您希望有权访问自定义视图的用户的名称或电子邮件地址，然后在下拉列表中显示该名称时单击该名称。
   * 如果您此时选择不与其他用户共享您的视图，则以后可以通过编辑自定义视图来共享。

1. 单击&#x200B;**[!UICONTROL 创建]**。
1. 此时将显示“自定义”视图，该视图可在 [!DNL Views] 页面。 有关视图的更多信息，请参阅 [管理 [!DNL Views] 页面 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

## 编辑自定义视图

您可以轻松编辑自定义视图。 要编辑自定义视图，请执行以下操作：

1. 转到 **[!UICONTROL 视图]** 页面。\
   有关视图的更多信息，请参阅 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. 单击 [!UICONTROL 视图] 按钮(1)
1. 从下拉菜单中选择要编辑的视图。\
   ![](assets/proof-view-edit.png)

1. 单击 **[!UICONTROL 查看选项]** 按钮，然后单击 **[!UICONTROL 编辑视图]**.\
   ![](assets/proof-view-options.png)\
   此时将显示“编辑自定义视图”页面。

1. 单击 [!UICONTROL 操作] 菜单。 (3)\
   仅当视图中包含校样名称列时，此按钮才可用。
1. 选择 [!UICONTROL 编辑视图] 中。 (4) \
   ![editing_custom_view_2.png](assets/editing-custom-view-2-350x258.png)

1. 此时将显示“编辑自定义视图”页面。

![Edit_custom_view_page.png](assets/edit-custom-view-page-350x543.png)

>[!NOTE]
>
>如果编辑“自定义”视图，则“选定的列”列表中的列将自动按字母顺序排列。 在更新视图之前，您需要根据需要重新排列它们。


## 复制自定义视图

使用“复制”视图功能，您可以轻松复制现有的自定义视图。 例如，如果您要为所有设计人员设置单独的视图，并且除校样所有者（设计人员）之外，每个视图都是相同的，这非常有用。

要复制自定义视图，请执行以下操作：

1. 转到 **[!UICONTROL 视图]** 页面。\
   有关视图的更多信息，请参阅 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. 单击 **[!UICONTROL 视图]** 按钮。 (1)
1. 从列表中选择您的自定义视图。 (2)
1. 单击 **[!UICONTROL 操作]** 菜单。 (3)\
   仅当视图中包含校样名称列时，此按钮才可用。

1. 选择 [!UICONTROL 复制] 中。 (4)\
   ![copying_custom_view.png](assets/copying-custom-view-350x258.png)

1. 在“复制自定义视图”页面中，将填充所有原始设置。 根据您的选择修改自定义视图，然后单击 **[!UICONTROL 复制视图]** 按钮。 您将立即转到新视图。\
   ![](assets/copy-custom-view-page-350x542.png)

## 共享自定义视图

如果您尚未在视图的“共享”部分选择共享视图，则使用“共享视图”功能可以与帐户中的其他用户共享视图。 当您与其他用户共享自定义视图时，该视图会显示在其 [!UICONTROL 我的自定义视图] 的子菜单。

要与其他用户共享自定义视图，请执行以下操作：

1. 转到 **[!UICONTROL 视图]** 页面。\
   有关视图的更多信息，请参阅 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. 单击 **[!UICONTROL 视图]** 按钮(1)
1. 从列表中选择自定义视图(2)
1. 单击 **[!UICONTROL 操作]** 菜单。 (3)\
   仅当视图中包含校样名称列时，此按钮才可用。

1. 选择 [!UICONTROL 共享视图] 菜单(4)
1. 此时将显示“编辑自定义视图”页面。
1. 在 [!UICONTROL 共享] 部分选择要与之共享视图的用户，然后单击 **[!UICONTROL 更新视图]**.

   ![Edit_custom_view_page__1_.png](assets/edit-custom-view-page--1--350x543.png)

## 将自定义视图导出为CSV文件

要将数据从自定义视图导出到CSV文件，请执行以下操作：

1. 转到 **[!UICONTROL 视图]** 页面。\
   有关视图的更多信息，请参阅 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. 单击 **[!UICONTROL 视图]** 按钮。 (1)
1. 从列表中选择您的自定义视图。 (2)
1. 单击 **[!UICONTROL 操作]** 菜单。 (3)\
   仅当视图中包含校样名称列时，此按钮才可用。

1. 选择 [!UICONTROL 导出到CSV] 中。 (4)\
   ![exporting_custom_view.png](assets/exporting-custom-view-350x258.png)\
   在单独的浏览器窗口中，“生成报表：显示“100%”加上记录数（自定义视图中报表中包含的项目数）

1. （视情况而定）如果出现安全消息，指示当前阻止了报告下载，请单击以允许下载继续。
1. 单击 **[!UICONTROL 保存]** 当出现“文件下载”窗口询问您是要打开还是保存文件时。
1. 选择计算机上的某个位置并保存文件。

## 删除自定义视图

您可以轻松删除自定义视图。 要执行此操作，请执行以下操作：

1. 转到 **[!UICONTROL 视图]** 页面。\
   有关视图的更多信息，请参阅 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. 单击 **[!UICONTROL 视图]** 按钮。
1. 从列表中选择自定义视图
1. 单击 **[!UICONTROL 操作]** 菜单。 (3)\
   仅当视图中包含校样名称列时，此按钮才可用。

1. 选择 [!UICONTROL 删除] 中。 (4)\
   ![deleting_custom_view.png](assets/deleting-custom-view-350x258.png)

1. 单击 **[!UICONTROL 删除]** (5)确认您要删除当前的“自定义”视图\
   ![delete__1_.png](assets/delete--1--350x187.png)

1. 将显示默认的“所有项目”视图，并且删除的自定义视图将不再显示在 **[!UICONTROL 视图]** 下拉菜单。
