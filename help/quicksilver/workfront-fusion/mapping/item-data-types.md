---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 中的项目数据类型 [!DNL Adobe Workfront Fusion]
description: 您的 [!DNL Adobe Workfront Fusion] 方案可以包含捆绑包中下面列出的项目类型。
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# 中的项目数据类型 [!DNL Adobe Workfront Fusion]

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
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
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

## 项目数据类型

可在捆绑包中包含下面列出的项目类型。

有关哪些项目类型的信息 [!DNL Workfront Fusion] 允许相互转换，请参阅 [键入强制 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>文本</p> </td> 
   <td> <p>最常见的项类型。 对于某些文本项， [!DNL Adobe Workfront Fusion] 检查是否满足允许的最大或最小长度，或者项目是否执行格式验证（电子邮件、URL或文件名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>数字</p> </td> 
   <td> <p>对于某些数值项， [!DNL Workfront Fusion] 可以验证指定范围（允许的最小值或最大值）的输入。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>布尔值（是/否）</p> </td> 
   <td> <p>此类型用于只有两个可能值的项目：true或false。 </p> <p>设置模块时，布尔类型可以有两种不同的形式：</p> 
    <ul> 
     <li> <p>如果字段为必填字段，且必须填写，则会显示必填复选框。</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>可留空的可选字段显示为选择框，允许从三个值中进行选择： <code>Yes</code>， <code>No</code>、和 <code>Not defined</code> （默认）。</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>您可以单击 <strong>[！UICONTROL映射]</strong> 如果需要将该值映射到另一个模块中的项，请执行以下操作。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>日期</p> </td> 
   <td> <p>日期以ISO 8601日期格式输入，例如， <code>2015-09-18T11:58Z</code>. 您可以在配置文件设置中更改时区，如中所述 <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">在中更改配置文件设置 [!DNL Adobe Workfront Fusion]</a>. </p> <p>如果单击需要日期的字段，则模块设置中会显示一个弹出日历。 某些项目不需要时间。</p> <p>日期项目的值使用在您的配置文件中选择的本地和Web时区进行格式化。 通过将鼠标悬停在某个日期项上，可以显示该日期项值的ISO 8601版本。</p> <p>注意：如果ISO值未显示，则该项目可能是文本，而不是日期。</p> <p>时间输入于 <code>hours:minutes:seconds</code> 格式，例如，<code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>缓冲区（二进制数据）</p> </td> 
   <td> <p>文件内容通常作为缓冲区类型内容（图像内容、视频文件等）发送。 在某些情况下，文本数据包含在此类型中（例如，文本文件）。 [!DNL Workfront Fusion] 能够自动将二进制代码中的文本数据转换为文本，将文本数据转换为二进制代码中的文本数据。 有关更多信息，请参阅 <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">关于在[！UICONTROL Adobe Workfront Fusion]中映射文件</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>收藏集</p> </td> 
   <td> <p>收藏集是由多个子项目组成的项目。 电子邮件中的“发件人”项目是集合的一个示例：它包含发件人姓名（文本类型）和发件人电子邮件地址（文本类型）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>选择（菜单）</p> </td> 
   <td> <p>配置模块设置时（如所述） <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">在中配置模块的设置 [!DNL Adobe Workfront Fusion]</a>，您可以从多个相同类型的项目中进行选择。 例如，的设置中的文件夹选择菜单 [!DNL Dropbox] 模块。 </p> <p>设置模块时，“选择”菜单可能以两种形式出现：</p> <p> <p>如果可以进行多选，则会显示多个包含复选框的项目。</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>如果只有一个选项，则会显示下拉菜单。</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>如果需要从另一个模块映射项目，请使用 <strong>映射</strong> 按钮。 此按钮将打开一个文本字段而不是选择菜单。 有关更多信息，请参阅 <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>数组</p> </td> 
   <td> <p>您可以使用数组类型来处理多个相同类型的值，包括集合。 [！UICONTROL Email]模块就是一个例子：它们返回一个附件数组，每个附件都包含名称、内容、大小等。 有关更多信息，请参阅 <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">映射数组 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>验证</p> </td> 
   <td> <p>[!DNL Workfront Fusion] 可能会对每种类型的项目执行验证。 如果项目未通过验证，则模块将因数据错误而停止处理。 有关更多信息，请参阅 <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">处理以下对象时出错： [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
