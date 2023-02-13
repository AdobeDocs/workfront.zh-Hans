---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用OneDrive的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 13a25c6c-bdf1-467d-bd90-ebd763c59235
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3934'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL OneDrive]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!DNL OneDrive] 模块，您必须 [!DNL Microsoft OneDrive] 帐户。

## 连接 [!DNL OneDrive] 服务 [!DNL Workfront Fusion]

有关连接 [!DNL OneDrive] 帐户 [!UICONTROL Workfront Fusion]，请参阅 [创建连接 [!UICONTROL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive] 模块及其字段

配置 [!DNL OneDrive] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL OneDrive] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [文件/文件夹](#filefolder)
* [其他](#other)

### 文件/文件夹

* [[!UICONTROL 监视文件/文件夹]](#watch-filesfolders)
* [[!UICONTROL 搜索文件/文件夹]](#search-filesfolders)
* [[!UICONTROL 获取文件]](#get-a-file)
* [[!UICONTROL 下载文件]](#download-a-file)
* [[!UICONTROL 上传文件]](#upload-a-file)
* [[!UICONTROL 创建文件夹]](#create-a-folder)
* [[!UICONTROL 获取共享链接]](#get-a-share-link)
* [[!UICONTROL 移动文件/文件夹]](#move-a-filefolder)
* [[!UICONTROL 复制文件]](#copy-a-file)
* [[!UICONTROL 删除文件/文件夹]](#delete-a-filefolder)

#### [!UICONTROL 监视文件/文件夹]

创建或更新文件或文件夹后，此触发器模块会启动一个方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td>有关连接 [!DNL OneDrive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL监视文件/文件夹]</td> 
   <td> <p>选择您希望如何监视文件或文件夹：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL By Created Time]</b> </p> <p>监视新文件或文件夹。</p> </li> 
     <li> <p><b>[!UICONTROL By Updated Time]</b> </p> <p>监视已更新的现有文件或文件夹。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>选择要监视的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>选择是否启用模块以输入驱动器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>输入您希望模块监视的驱动器ID。</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>导航到您希望模块监视的文件夹。 您还可以输入查询以筛选返回的结果。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！与我共享的UICONTROL]</b> </p> <p>模块会监视已与驱动器所有者共享的文件。</p> </li> 
     <li> <p><b>[!UICONTROL Site的驱动器]</b> </p> <p>选择您希望模块监视的SharePoint网站。 可用站点是站点，后跟登录用户。</p> </li> 
     <li> <p><b>[!UICONTROL组的驱动器]</b> </p> <p>选择您希望模块监视其驱动器的组。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择项目类型]</td> 
   <td> <p>选择您是要监视文件、文件夹，还是同时监视两者。</p> <p>注意：您无法在[!UICONTROL与我共享]驱动器中监视文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>



#### [!UICONTROL 搜索文件/文件夹]

此搜索模块会根据您设置的条件返回文件和文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td>有关连接 [!DNL OneDrive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>选择要搜索的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>选择是否启用模块以输入驱动器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>输入您希望模块搜索的驱动器ID。</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>导航到您希望模块搜索的文件夹。 您还可以输入查询以筛选返回的结果。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！与我共享的UICONTROL]</b> </p> <p>模块会搜索与驱动器所有者共享的文件。</p> </li> 
     <li> <p><b>[!UICONTROL Site的驱动器]</b> </p> <p>选择 [!DNL SharePoint] 您希望模块搜索的网站。 可用站点是站点，后跟登录用户。</p> </li> 
     <li> <p><b>[!UICONTROL组的驱动器]</b> </p> <p>选择要模块搜索其驱动器的组。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择项目类型]</td> 
   <td> <p>选择是要搜索文件、文件夹，还是同时搜索两者。</p> <p>注意：您无法在[!UICONTROL与我共享]驱动器中搜索文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

此操作模块获取指定文件的元数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td>有关连接 [!DNL OneDrive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter（文件ID和文件路径）]</td> 
   <td>选择是要按文件ID还是按文件路径来标识文件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入文件ID] / [!UICONTROL文件路径]</td> 
   <td> <p>选择输入文件ID或文件路径的方式：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手动输入]</b> </p> <p>如果要直接输入ID或路径，或从上一个模块映射ID或路径，请选择此选项。</p> </li> 
     <li> <p><b>[!UICONTROL从列表中选择]</b> </p> <p>如果要从可用文件或路径的列表中进行选择，请选择此选项。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>选择要搜索的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>选择是否启用模块以输入驱动器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>输入包含要获取的文件的驱动器的ID。</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site的驱动器]</b> </p> <p>选择包含要获取的文件的SharePoint网站。 可用站点是站点，后跟登录用户。</p> </li> 
     <li> <p><b>[!UICONTROL组的驱动器]</b> </p> <p>选择其驱动器包含要获取的文件的组。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驱动器ID]</td> 
   <td> <p>选择或映射包含要获取的文件的驱动器。 如果您在[!UICONTROL启用以输入驱动器ID]字段中选择了[!UICONTROL No]，则此字段不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件] / [!UICONTROL文件ID] / [!UICONTROL文件路径]</td> 
   <td> <p>如果您选择了[!UICONTROL Enter Manually]，请输入或映射要获取的文件的文件ID或路径。</p> <p>如果您选择了[!UICONTROL从列表中选择]，请选择要获取的文件。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下载文件]

此操作模块下载指定的文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td>有关连接 [!DNL OneDrive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter（文件ID和文件路径）]</td> 
   <td>选择是要按文件ID还是按文件路径来标识文件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">输入文件ID /文件路径</td> 
   <td> <p>选择输入文件ID或文件路径的方式：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手动输入]</b> </p> <p>如果要直接输入ID或路径，或从上一个模块映射ID或路径，请选择此选项。</p> </li> 
     <li> <p><b>[!UICONTROL从列表中选择]</b> </p> <p>如果要从可用文件或路径的列表中进行选择，请选择此选项。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>选择要包含要下载文件的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>选择是否启用模块以输入驱动器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>输入包含要下载文件的驱动器的ID。</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site的驱动器]</b> </p> <p>选择包含要下载的文件的SharePoint网站。 可用站点是站点，后跟登录用户。</p> </li> 
     <li> <p><b>[!UICONTROL组的驱动器]</b> </p> <p>选择要下载其驱动器所在的组。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驱动器ID]</td> 
   <td> <p>选择或映射包含要下载文件的驱动器。 如果您在[!UICONTROL启用以输入驱动器ID]字段中选择了[!UICONTROL No]，则此字段不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件] / [!UICONTROL文件ID] / [!UICONTROL文件路径]</td>
   <td> <p>如果您选择了[!UICONTROL Enter Manually]，请输入或映射要下载的文件的文件ID或路径。</p> <p>如果您选择了[!UICONTROL从列表中选择]，请选择要下载的文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL转换为PDF]</td> 
   <td> <p>启用此选项可将文件转换为PDF文件。 您可以从以下文件类型进行转换：</p> 
    <table style="table-layout:auto"> 
     <col> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td> 
        <ul> 
         <li> <p> <p>CSV</p> </p> </li> 
         <li> <p> <p>文档</p> </p> </li> 
         <li> <p> <p>DOCX</p> </p> </li> 
         <li> <p> <p>ODP</p> </p> </li> 
         <li> <p> <p>ODS</p> </p> </li> 
         <li> <p> <p>ODT</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p> <p>锅</p> </p> </li> 
         <li> <p> <p>POTM</p> </p> </li> 
         <li> <p> <p>POTX</p> </p> </li> 
         <li> <p> <p>PPS</p> </p> </li> 
         <li> <p> <p>PPSX</p> </p> </li> 
         <li> <p> <p>PPSXM</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p>PPT</p> </li> 
         <li> <p>PPTM</p> </li> 
         <li> <p>PPTX</p> </li> 
         <li> <p>RTF</p> </li> 
         <li> <p>XLS</p> </li> 
         <li> <p>XLSX</p> </li> 
        </ul> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上传文件]

此操作模块将文件上传到指定的文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td>有关连接 [!DNL OneDrive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">输入（文件夹位置ID和路径）</td> 
   <td>选择您是要按ID还是路径来标识目标文件夹。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>选择要上传文件的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>选择是否启用模块以输入驱动器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>选择包含要获取的文件的驱动器。</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site的驱动器]</b> </p> <p>选择 [!DNL SharePoint] 包含要上传文件的文件夹的网站。 可用站点是站点，后跟登录用户。</p> </li> 
     <li> <p><b>[!UICONTROL组的驱动器]</b> </p> <p>选择其驱动器包含要上传文件的文件夹的组。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驱动器ID]</td> 
   <td> <p>选择包含要上传文件的文件夹的驱动器。 如果您在[!UICONTROL启用以输入驱动器ID]字段中选择了[!UICONTROL No]，则此字段不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL如果存在同名文件]</td> 
   <td>如果已存在同名文件，请选择如何继续。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL描述]</td> 
   <td>向上传的文件添加描述。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建文件夹]

此操作模块在指定的驱动器中创建新文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td>有关连接 [!DNL OneDrive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>选择要创建文件夹的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>选择是否启用模块以输入驱动器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>选择要创建文件夹的驱动器。</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site的驱动器]</b> </p> <p>选择 [!DNL SharePoint] 要创建文件夹的网站。 可用站点是站点，后跟登录用户。</p> </li> 
     <li> <p><b>[!UICONTROL组的驱动器]</b> </p> <p>选择要创建文件夹的驱动器的所有者组。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驱动器ID]</td> 
   <td> <p>选择要创建文件夹的驱动器。 如果您在[!UICONTROL启用以输入驱动器ID]字段中选择了[!UICONTROL No]，则此字段不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件夹]</td> 
   <td>如果希望新文件夹是子文件夹，请导航到您希望该文件夹成为其子文件夹的文件夹。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL新文件夹名称]</td> 
   <td> <p>输入或映射新文件夹的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL如果存在同名文件夹]</td> 
   <td>如果已存在同名文件，请选择如何继续。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取共享链接]

此操作模块会返回指定文件的共享链接。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td>有关连接 [!DNL OneDrive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter（文件ID和文件路径）]</td> 
   <td>选择是要按文件ID还是按文件路径来标识文件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入文件ID] / [!UICONTROL文件路径]</td> 
   <td> <p>选择输入文件ID或文件路径的方式：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手动输入]</b> </p> <p>如果要直接输入ID或路径，或从上一个模块映射ID或路径，请选择此选项。</p> </li> 
     <li> <p><b>[!UICONTROL从列表中选择]</b> </p> <p>如果要从可用文件或路径的列表中进行选择，请选择此选项。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>选择要检索共享链接的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>选择是否启用模块以输入驱动器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>输入包含要检索其共享链接的文件的驱动器ID。</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site的驱动器]</b> </p> <p>选择包含要检索其共享链接的文件的SharePoint网站。 可用站点是站点，后跟登录用户。</p> </li> 
     <li> <p><b>[!UICONTROL组的驱动器]</b> </p> <p>选择其驱动器包含要检索其共享链接的文件的组。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驱动器ID]</td> 
   <td> <p>选择或映射包含要检索其共享链接的文件的驱动器。 如果您在[!UICONTROL启用以输入驱动器ID]字段中选择了[!UICONTROL No]，则此字段不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件] / [!UICONTROL文件ID] / [!UICONTROL文件路径]</td> 
   <td> <p>如果您选择[!UICONTROL Enter Manually]，请输入或映射要检索其共享链接的文件的文件ID或路径。</p> <p>如果从列表中选择[!UICONTROL Select]，请选择要检索其共享链接的文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL权限类型]</td> 
   <td> <p>选择希望具有链接的人员能够读取和写入文件，还是只读。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL范围]</td> 
   <td>选择您希望该文件可供具有链接的任何人使用，还是仅供具有链接的组织成员使用。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移动文件/文件夹]

此操作模块将文件或文件夹移动到新文件夹位置

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td>有关连接 [!DNL OneDrive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter（文件ID和文件路径）]</td> 
   <td>选择是要按文件ID还是按文件路径来标识文件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入文件ID /文件路径]</td> 
   <td> <p>选择输入文件ID或文件路径的方式：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手动输入]</b> </p> <p>如果要直接输入ID或路径，或从上一个模块映射ID或路径，请选择此选项。</p> </li> 
     <li> <p><b>[!UICONTROL从列表中选择]</b> </p> <p>如果要从可用文件或路径的列表中进行选择，请选择此选项。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>选择包含要移动的文件或文件夹的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>选择是否启用模块以输入驱动器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>输入包含要移动的文件或文件夹的驱动器ID。</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site的驱动器]</b> </p> <p>选择 [!DNL SharePoint] 包含要移动的文件或文件夹的网站。 可用站点是站点，后跟登录用户。</p> </li> 
     <li> <p><b>[!UICONTROL组的驱动器]</b> </p> <p>选择要移动的文件或文件夹所在的组。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驱动器ID]</td> 
   <td> <p>选择或映射包含要移动的文件或文件夹的驱动器。 如果您在[!UICONTROL启用以输入驱动器ID]字段中选择了[!UICONTROL No]，则此字段不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">选择[!UICONTROL File/Folder]</td> 
   <td>选择要移动文件还是文件夹。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL文件] / [!UICONTROL文件ID] / [!UICONTROL文件路径]</p> <p role="rowheader">[!UICONTROL文件夹] / [!UICONTROL文件夹ID] / [!UICONTROL文件夹路径]</p> </td> 
   <td> <p>如果您选择了[!UICONTROL手动输入]，请输入或映射要移动的文件或文件夹的ID或路径。</p> <p>如果从列表中选择[!UICONTROL Select]，请选择要移动的文件或文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入新文件夹位置]</td> 
   <td> <p>选择要输入要将文件或文件夹移动到的位置的方式：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手动输入]</b> </p> <p>如果要直接输入ID或路径，或从上一个模块映射ID或路径，请选择此选项。</p> </li> 
     <li> <p><b>[!UICONTROL从列表中选择]</b> </p> <p>如果要从可用文件或路径的列表中进行选择，请选择此选项。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>选择要移动文件或文件夹的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>选择是否启用模块以输入驱动器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>输入要移动文件或文件夹的驱动器ID。</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site的驱动器]</b> </p> <p>选择 [!DNL SharePoint] 要移动文件或文件夹的站点。 可用站点是站点，后跟登录用户。</p> </li> 
     <li> <p><b>[!UICONTROL组的驱动器]</b> </p> <p>选择要将文件或文件夹移动到其驱动器的组。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驱动器ID]</td> 
   <td> <p>选择或映射包含要将文件或文件夹移动到的文件夹的驱动器。 如果您在[!UICONTROL启用以输入驱动器ID]字段中选择了[!UICONTROL No]，则此字段不可用。</p> <p>如果将此选项留空，则只能在同一个文件或文件夹中移动 [!DNL OneDrive].</p> <p>您可以将文件和文件夹从[!UICONTROL My Drive]移动到[!UICONTROL站点的驱动器]或[!UICONTROL组的驱动器]。 </p> <p>您只能将文件从[!UICONTROL站点的驱动器]移动到同一站点中的同一驱动器。</p> <p>您只能将文件从[!UICONTROL组的驱动器]移动到同一组中的同一驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件夹]</td> 
   <td>输入或映射要移动文件或文件夹的文件夹。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 复制文件]

此操作模块将文件复制到新文件夹位置

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td>有关连接 [!DNL OneDrive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter（文件ID和文件路径）]</td> 
   <td>选择是要按文件ID还是按文件路径来标识文件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入文件ID] / [!UICONTROL文件路径]</td> 
   <td> <p>选择输入文件ID或文件路径的方式：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手动输入]</b> </p> <p>如果要直接输入ID或路径，或从上一个模块映射ID或路径，请选择此选项。</p> </li> 
     <li> <p><b>[!UICONTROL从列表中选择]</b> </p> <p>如果要从可用文件或路径的列表中进行选择，请选择此选项。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>选择包含要复制的文件的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>选择是否启用模块以输入驱动器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>输入包含要复制的文件或文件夹的驱动器ID。</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site的驱动器]</b> </p> <p>选择包含要移动的文件的SharePoint网站。 可用站点是站点，后跟登录用户。</p> </li> 
     <li> <p><b>[!UICONTROL组的驱动器]</b> </p> <p>选择驱动器包含要复制的文件的组。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驱动器ID]</td> 
   <td> <p>选择或映射包含要复制的文件的驱动器。 如果您在[!UICONTROL启用以输入驱动器ID]字段中选择了[!UICONTROL No]，则此字段不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL文件] / [!UICONTROL文件ID] / [!UICONTROL文件路径]</p> </td> 
   <td> <p>如果您选择了[!UICONTROL Enter Manually]，请输入或映射要复制的文件的ID或路径。</p> <p>如果从列表中选择[!UICONTROL Select]，请选择要复制的文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入新文件夹位置]</td> 
   <td> <p>选择要输入要复制文件或要复制到的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手动输入]</b> </p> <p>如果要直接输入ID或路径，或从上一个模块映射ID或路径，请选择此选项。</p> </li> 
     <li> <p><b>[!UICONTROL从列表中选择]</b> </p> <p>如果要从可用文件夹列表中进行选择，请选择此选项。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL新OneDrive位置]</td> 
   <td> <p>选择要复制文件管理器的位置。 如果您选择从列表中选择新文件夹位置，则此选项将可用。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>选择是否启用模块以输入驱动器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>输入要将文件复制到的驱动器的ID。</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site的驱动器]</b> </p> <p>选择 [!DNL SharePoint] 要复制文件的站点。 可用站点是站点，后跟登录用户。</p> </li> 
     <li> <p><b>[!UICONTROL组的驱动器]</b> </p> <p>选择要将文件复制到其驱动器的组。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驱动器ID]</td> 
   <td> <p>选择或映射包含要将文件复制到的文件夹的驱动器。 如果您在[!UICONTROL启用以输入驱动器ID]字段中选择了[!UICONTROL No]，则此字段不可用。</p> <p>如果将此留空，则只能在同一[!UICONTROL OneDrive]内复制文件或文件夹。</p> <p>您可以将文件和文件夹从[!UICONTROL My Drive]复制到[!UICONTROL站点的驱动器]或[!UICONTROL组的驱动器]。 </p> <p>您只能将文件从[!UICONTROL站点的驱动器]复制到同一站点中的同一驱动器。</p> <p>您只能将文件从[!UICONTROL组的驱动器]复制到同一组中的同一驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件夹]</td> 
   <td>输入或映射要移动副本或文件夹的文件夹。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New Copied File Name]</td> 
   <td> <p>输入或映射文件新副本的名称。 如果不想更改原始文件名，可将此字段留空。</p> <p>名称必须包含文件扩展名。 示例:<code> file.txt</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件/文件夹]

此操作模块将删除所选文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td>有关连接 [!DNL OneDrive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter（文件/文件夹ID和路径）]</td> 
   <td>选择是要按文件ID还是按文件路径来标识文件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入文件/文件夹ID /输入文件/文件夹路径]</td> 
   <td> <p>选择输入文件ID或文件路径的方式：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手动输入]</b> </p> <p>如果要直接输入ID或路径，或从上一个模块映射ID或路径，请选择此选项。</p> </li> 
     <li> <p><b>[!UICONTROL从列表中选择]</b> </p> <p>如果要从可用文件或路径的列表中进行选择，请选择此选项。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>选择要搜索的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>选择是否启用模块以输入驱动器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>输入包含要删除的文件或文件夹的驱动器ID。</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site的驱动器]</b> </p> <p>选择 [!DNL SharePoint] 包含要删除的文件或文件夹的网站。 可用站点是站点，后跟登录用户。</p> </li> 
     <li> <p><b>[!UICONTROL组的驱动器]</b> </p> <p>选择其驱动器包含要删除的文件或文件夹的组。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驱动器ID]</td> 
   <td> <p>选择或映射包含要删除的文件或文件夹的驱动器。 如果您在[!UICONTROL启用以输入驱动器ID]字段中选择了[!UICONTROL No]，则此字段不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">选择[!UICONTROL File/Folder]</td> 
   <td>选择要删除文件还是文件夹。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件] / [!UICONTROL文件ID] / [!UICONTROL文件路径]</td>
   <td> <p>如果您选择了[!UICONTROL手动输入]，请输入或映射要删除的文件的文件ID或路径。</p> <p>如果从列表中选择[!UICONTROL Select]，请选择要删除的文件。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

#### [!UICONTROL 进行API调用]

此模块执行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td>有关连接 [!DNL OneDrive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>输入相对于 <code>https://graph.microsoft.com</code>. 示例:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion会为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:  <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



## 如果您无法上传或更新文件

上传或更新文件失败时，可能会出现以下几个问题：

* 上传的文件太大，超出了 [!DNL OneDrive] 计划，或者你用了 [!DNL OneDrive] 帐户的存储配额。 要获取更多存储空间，请从 [!DNL OneDrive] 升级 [!DNL OneDrive] 帐户。
* OneDrive不允许将两个同名文件上载到一个文件夹。 如果目标文件夹包含的文件与上传的文件同名，则运行方案将终止，并出现错误。 解决方案是只需对上传的文件进行重命名即可。 如果您的目标是更新文件，请使用 [!UICONTROL 更新文件] 操作。
* 之前选择的文件夹（正在将文件上传到的文件夹）不再存在。 方案停止，您将需要再次选择目标文件夹。
