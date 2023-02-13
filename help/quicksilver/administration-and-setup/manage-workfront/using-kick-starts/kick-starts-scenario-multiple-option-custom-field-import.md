---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart，kickstart，kickstarts，kickstarts
navigation-topic: use-kick-starts
title: ‘启动方案：将多选项自定义字段导入Workfront
description: 您可以使用“Kick-Start”功能在Adobe Workfront中导入包含多个选项的自定义字段。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 80ad604330e8b55037f1607b754cc8bb34f6a3ec
workflow-type: tm+mt
source-wordcount: '2126'
ht-degree: 0%

---


# “启动”方案：将多选项自定义字段导入Workfront

您可以使用“Kick-Start”功能在Adobe Workfront中导入包含多个选项的自定义字段。

具有多个选项的自定义字段示例包括：

* 多选下拉框
* 下拉
* 复选框
* 单选按钮

这些字段有时可以有许多（有时是数百个）选项。 使用Kick-Start功能导入它们可以节省您(作为Workfront管理员)大量时间并确保避免出现错误。

>[!IMPORTANT]
>
>您必须按照以下各节中所述的步骤，依次使用启动导入包含多个选项的自定义字段：
>
>1. 从Workfront导出现有自定义数据（可选步骤）
>1. 导出自定义数据的启动模板
>1. 填充Excel Kick-Starts电子表格
>1. 将Excel电子表格上传到Workfront



## 从Workfront导出现有自定义数据（可选步骤）

如果您不熟悉Workfront数据库结构，或者您不熟悉Workfront导入信息所需的启动文件，我们建议您首先从Workfront导出一个包含现有信息的启动文件，与要导入的字段类似。

例如，如果要导入自定义表单或自定义字段，则必须先导出具有现有自定义数据的启动文件。

首先导出现有数据允许您扫描该数据，并了解新数据的格式设置。

如果您对Workfront数据库对象和结构有很好的了解，可以继续下面的部分。

要从Workfront导出现有数据，请执行以下操作：

1. 单击 **主菜单>设置** 中找到。
1. 展开 **系统** 菜单，然后单击 **导出数据（启动）**.

   ![](assets/export-data-kick-starts-link-in-setup.png)

1. 选择 **自定义数据** 在 **要包含的内容** 中。

   ![](assets/existing-custom-data-box-checked-kick-starts.png)

1. 选择 **.xlsx文件** 在 **下载格式** 中。

   >[!TIP]
   >
   >    根据您在系统中拥有的自定义数据量，这可能需要很长时间。

   ![](assets/download-button-for-kick-starts.png)

1. 单击 **下载**. .xlsx文件将下载到您的计算机。 导航到并将其打开。

   ![](assets/existing-data-excel-parameter-sheet.png)

1. 检查下载的文件，并记下以下详细信息：

   * 文件包含多个工作表。 您可能不需要知道每个工作表中的信息，但是您会使用其中的一些工作表来导入信息。 请花些时间熟悉其内容，特别是每个工作表中内容的格式。
   * 请特别注意列名称以及每列中显示数据的格式。
   * 不得更改任何工作表中列的名称或顺序。 列标题指示您需要在每个行中填写其信息的字段。 如果列标题以粗体显示，则它是必填字段，因此您必须在该列中包含信息。
   >[!IMPORTANT]
   >
   >某些列标题可能不会以粗体显示，但可能仍需要使用。

   * 保留下载的文件以供将来参考，并继续执行以下部分。


## 导出自定义数据的启动模板

扫描系统中现有自定义字段的相关信息后，您可以下载新的启动模板以供导入。

1. 单击 **主菜单>设置** 中找到。

1. 展开 **系统** 菜单。

1. 单击 **导入数据（启动）**.

   ![](assets/import-data-kick-starts-link-in-setup.png)

1. 在 **下载空白的Kick-Start电子表格** 区域，选择 **自定义数据** 复选框，单击 **下载**.

   ![](assets/blank-custom-data-option-checked-kick-starts.png)

   将启动文件下载到您的计算机时显示空白。

   >[!NOTE]
   >
   >文件中的工作表数、其名称以及每个工作表中列的数量和名称，应当与上节中下载的包含现有自定义数据的启动启动中下载的工作表的数量相同。

## 填充Excel Kick-Starts电子表格

在填充Excel电子表格之前，请按照上节所述下载启动模板。

>[!IMPORTANT]
>
>请勿尝试使用临时Excel电子表格导入信息。 所有使用启动功能将信息导入Workfront的电子表格都必须与您从Workfront下载并在本文中描述的文件内容相匹配。

要使用新自定义字段的信息填充Excel电子表格，请执行以下操作：

1. 打开您在上一部分中下载的Excel电子表格，并注意到许多工作表。 每个工作表表示应用程序中的一个对象。

   >[!INFO]
   >
   >例如， **参数** （指自定义字段）， **参数选项**（这是指“自定义字段”选项）， **类别** （指自定义表单）。
   >
   >必须以Workfront数据库支持的格式写入对象的名称及其属性。
   >
   >有关这些对象含义的信息，请参阅 [Workfront术语表](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
   >
   >有关Workfront数据库中对象名称的信息，请参阅 [API Explorer](../../../wf-api/general/api-explorer.md).
   >
   >![](assets/sheets-included-in-custom-data-export-kick-start-file.png)





1. 确保以下信息的格式正确：

   * 每个工作表的第一行必须留空，否则，导入会生成错误。
   * 每个工作表中的列标题表示可在导入期间设置的对象的属性。 导出工作表时，所有列标题必须保持您找到它们的相同顺序，并且不能重命名。
   * 以粗体显示的列标题是必填字段，且必须具有值。

      >[!TIP]
      >
      >某些列不是粗体列，但是它是必需的。 例如， `isNew` 和 `ID` 列不是粗体，但是它们是必填字段。

1. 选择 `**PARAM Parameter`**工作表，并在以下必需列中添加有关新自定义字段的信息：

   * **`isNew`** = enter **`TRUE`** 在此列中，每个表示新自定义字段的行均对应。 这表示该字段是新字段，且不存在于Workfront中。

      >[!TIP]
      >
      >    如果行表示Workfront中已有的字段，则您应输入 **`isNew`** = **`FALSE`**.

   * **`ID`** =必须为表示新字段的每行的唯一数字。 只要每个新字段都有唯一的数字，您就可以使用以1开头的任意数字。
   * **`setDataType`** =对于表示新字段的每行，输入字段支持的数据类型。 必须按数据库中显示的方式输入数据类型。 从以下数据类型中进行选择：
      * **`NMBR`** 表示数字
      * **`CURC`** （货币）
      * **`TEXT`** （文本）
   * `**setDisplaySize**`=显示大小(&#39;**setDisplaySize**“)对于任何多个选项，自定义字段始终为0。
   * **`setDisplayType`** =对于表示新字段的每行，输入字段的显示类型。 必须输入显示类型，该类型将显示在数据库中。

      对于多选项自定义字段，请从以下选项中选择：

      * **`MULT`** （对于多选下拉列表）
      * **`SLCT`** （表示下拉列表）
      * **`RDIO`** （表示单选按钮）
      * **`CHCK`** 复选框
      >[!TIP]
      >
      >要查找数据类型和显示类型信息，请参阅 [API Explorer](../../../wf-api/general/api-explorer.md)，展开 **参数** 对象，并在下方查找这些属性 **字段** 选项卡。

   * **`setName`** =输入您希望在Workfront中显示的自定义字段名称。

      >[!INFO]
      >
      >例如，我们可能会导入两个自定义字段，称为 _品牌_&#x200B;复选框字段和 _媒体_，单选按钮字段。

   * 的 **`setName`** 和 **`setValue`** 列通常包含相同的信息，它们应反映新字段在Workfront界面中所需的名称。
   例如，字段的值是报表中显示的名称，而名称显示在附加到对象的自定义表单中。

   有关更多信息，请参阅 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).

   ![](assets/parameter-sheet-filled-out-kick-starts.png)

1. 选择 **`POPT Parameter Options`** 工作表并在以下必需列中添加有关每个自定义字段选项的信息：

   * **`isNew`** = enter **`TRUE`** 在此列中，每个表示新字段选项的行均使用。

      >[!TIP]
      >
      >    如果行表示现有选项，则需输入 **`isNew`** = **`FALSE`**.

   * **`ID`** =必须为表示新选项的每行的唯一数字。 只要每个新选项具有唯一的数字，您就可以使用以1开头的任意数字。
   * **`setIsDefault`** = enter `TRUE` ，以及 `FALSE` ，用于每个字段。  例如，我们希望 _耐克_ 为 _品牌_ 和 _打印_ 为 _媒体_.

      >[!TIP]
      >
      >每个字段只能有一个默认选项。

   * **`setParameterID`** =对应于 _品牌_ 自定义字段具有 **`setParameterID`** 1，而与 _媒体_ 有个**`setParameterID`**/2. 的 `PARAM` 和 `POPT` 工作表相互交叉引用以指示哪些选项属于哪个自定义字段。
   * **`setDisplayOrder`**=显示顺序列指示选项在自定义字段中显示的顺序。 无论选项属于哪些字段，您都可以从1开始，并以升序方式继续运行所有选项。 这里的重要内容是，每个选项都具有唯一的数字。
   * 的 **`setLabel`** 和 `**setValue`**列通常包含相同的信息，它们应反映Workfront UI中所需的名称。 例如，选项的值是在报表中显示的名称，而标签在附加到对象后会显示在自定义表单中。 有关更多信息，请参阅 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
   * **`setIsHidden`** = enter `TRUE` 希望隐藏任何选项。
   ![](assets/parameter-option-sheet-filled-out-kick-starts.png)


1. （可选）如果还要创建一个自定义表单，以供您稍后添加新字段，请选择  **`CTGY Category`** 工作表并更新自定义表单信息的以下必需列：

   * **`isNew`** = enter **`TRUE`** 在此列中，表示新自定义表单的每一行对应。
   * **`ID`** =为每个表示新表单的行输入唯一数字。 只要每个新选项或新行都有唯一的编号，您就可以使用以1开头的任意编号。
   * **`setGroupID`** =为您的主组或系统中任何其他要拥有此表单访问权限的组的成员添加组ID。 这是必填字段。
   要了解 `ID` 组的报表，您可以生成群组报表并添加 `ID` 字段，或导航到某个群组并查找该群组的URL。 群组ID将位于群组页面的URL中。 例如，如果群组的URL为 `https://companyName.my.workfront.com/group/575b000800467a6f66e747932c807464/members`，组ID为 `575b000800467a6f66e747932c807464`.

   * **`setCatObjCode` **=这是您希望为其创建表单的对象类型的对象代码。 使用以下选项输入代码：
      * **`CMPY`** （对于公司）
      * **`TASK`** （任务）
      * **`PROJ`** （项目）
      * **`PORT`** Portfolio
      * **`PRGM`** （项目）
      * **`USER`** （用户）
      * **`DOCU`** （对于文档）
      * **`OPTASK`** （问题）
      * **`EXPNS`** （支出）
      * **`ITRN`** （小版本）
      * **`BILL`** 对于帐单记录
      * **`GROUP`** 对于组
      >[!NOTE]
      >
      >对于多对象表单，输入在UI中创建表单时要选择的第一个对象。 例如，将 `setCatObjCode` to `TASK`，但是您不希望该表单可用于项目。

   * **`setName`** =这是您希望在Workfront界面中显示的自定义表单名称。

      ![](assets/category-sheet-filled-out-kick-starts.png)



1. 将电子表格另存为.xls或.xlsx文件。 您的Excel电子表格已填写完毕，现已准备好导入Workfront。


## 将Excel电子表格上传到Workfront

执行前几节所述的步骤后，请继续执行以下步骤，将新字段和表单上传到Workfront:

1. 单击 **导入数据** **（开始）** **主菜单>设置>系统** 菜单。

1. 单击 **选择文件** 在部分下 **使用Kick-Start电子表格上传数据**.

1. 在您的计算机上浏览您准备的Excel电子表格，并在找到它时将其选中。  当Workfront识别文件时，“上传”按钮将变为蓝色。
1. 单击 **上传。**

   ![](assets/kick-start-file-selected-and-upload-blue-button.png)

1. 此时会显示导入成功的通知。 根据您正在导入的信息量，此步骤可能需要几秒钟到一分钟。

   ![](assets/kick-start-successful.png)

   新的自定义字段和表单现在位于您的Workfront系统中。 您可以在设置的自定义Forms区域中找到它们。

   >[!NOTE]
   >
   >新表单和导入的字段尚未连接。 导入的表单没有自定义字段。 您必须手动将字段添加到新的自定义表单或其他现有的自定义表单。


   有关向自定义表单添加字段的信息，请参阅 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).

1. （视情况而定）如果导入失败，您会收到一则错误消息，其中包含问题所在。 尝试识别遇到问题的字段、工作表和行号，并更正Excel文件中的信息，然后再尝试导入文件。

   ![](assets/kick-start-error.png)

1. （视情况而定）根据问题的内容（如错误消息中所述），可能已经导入了某些信息。 必须执行下列操作之一，才能再次导入工作表：

   * 从“自定义Forms”区域删除成功从Workfront导入的信息，然后进行错误消息指示的更正。
   * 指示系统中已导入的字段或表单的字段或表单已存在，然后进行更正。
要指示字段或自定义表单已在Workfront中，您必须确保 `inNew` 字段中的 `FALSE` 包含表单信息的工作表(`CTGY`)或字段(`PARAM`)。
