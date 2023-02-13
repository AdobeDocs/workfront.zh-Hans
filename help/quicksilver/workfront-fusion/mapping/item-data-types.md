---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 中的项目数据类型 [!DNL Adobe Workfront Fusion]
description: 您的 [!DNL Adobe Workfront Fusion] 方案可以包含捆绑包中列出的项目类型。
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# 中的项目数据类型 [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 项目数据类型

可以在包中包含下面列出的项目类型。

有关项目类型的信息 [!DNL Workfront Fusion] 允许彼此进行转换，请参阅 [在中键入强制 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>文本</p> </td> 
   <td> <p>最常见的项目类型。 对于某些文本项目， [!DNL Adobe Workfront Fusion] 检查是否满足允许的最大长度或最小长度，或项目是否执行格式验证（电子邮件、URL或文件名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>数字</p> </td> 
   <td> <p>对于一些数字项目， [!DNL Workfront Fusion] 可以验证指定范围（允许的最小或最大值）的输入。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>布尔值（是/否）</p> </td> 
   <td> <p>此类型用于仅具有两个可能值的项目：true或false。 </p> <p>设置模块时，布尔类型可以以两种不同的形式显示：</p> 
    <ul> 
     <li> <p>如果字段为必填字段且必须填写，则会显示强制复选框。</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>可留空的可选字段将显示为选择框，允许从以下三个值中进行选择： <code>Yes</code>, <code>No</code>和 <code>Not defined</code> （默认）。</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>您可以单击 <strong>[!UICONTROL映射]</strong> 如果您需要将值映射到其他模块中的项目。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>日期</p> </td> 
   <td> <p>日期以ISO 8601日期格式输入，例如， <code>2015-09-18T11:58Z</code>. 您可以在配置文件设置中更改时区，如 <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">更改 [!DNL Adobe Workfront Fusion]</a>. </p> <p>如果单击某个字段需要日期，则会在模块设置中显示一个弹出日历。 某些项目不需要时间。</p> <p>日期项的值使用配置文件中选择的本地和Web时区进行格式设置。 您可以通过将鼠标悬停在日期项目上来显示日期项目值的ISO 8601版本。</p> <p>注意：如果未显示ISO值，则项目可能是文本，而不是日期。</p> <p>时间在 <code>hours:minutes:seconds</code> 格式，例如，<code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>缓冲（二进制数据）</p> </td> 
   <td> <p>文件内容通常作为缓冲类型内容（图像内容、视频文件等）发送。 在某些情况下，文本数据会包含在此类型中（例如，文本文件）。 [!DNL Workfront Fusion] 能够自动将二进制代码中的文本数据转换为二进制代码中的文本数据和文本数据。 有关更多信息，请参阅 <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">关于在[!UICONTROL Adobe Workfront Fusion]中映射文件</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>收藏集</p> </td> 
   <td> <p>收藏集是包含多个子项目的项目。 电子邮件中的“发件人”项目是集合的一个示例：它包含发件人名称（文本类型）和发件人电子邮件地址（文本类型）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>选择（菜单）</p> </td> 
   <td> <p>按照 <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">在 [!DNL Adobe Workfront Fusion]</a>，则可以从多个相同类型的项目中进行选择。 例如， [!DNL Dropbox] 模块。 </p> <p>设置模块时，选择菜单可以以两种形式显示：</p> <p> <p>如果可以进行多个选择，则会显示多个带复选框的项目。</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>如果只能使用一个选项，则会显示下拉菜单。</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>如果您需要从其他模块映射项目，请使用 <strong>地图</strong> 按钮。 此按钮会打开一个文本字段而不是选择菜单。 有关更多信息，请参阅 <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">在 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>数组</p> </td> 
   <td> <p>您可以使用数组类型与多个相同类型的值（包括集合）一起使用。 例如，[!UICONTROL Email]模块：它们返回一个附件数组，每个附件都包含名称、内容、大小等。 有关更多信息，请参阅 <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">在中映射数组 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>验证</p> </td> 
   <td> <p>[!DNL Workfront Fusion] 可能会对每种类型的项目执行验证。 如果某个项目未通过验证，则模块将因数据错误而停止处理。 有关更多信息，请参阅 <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">处理中的错误 [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
