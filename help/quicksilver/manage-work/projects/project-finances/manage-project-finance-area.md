---
product-area: projects
navigation-topic: financials
title: 在项目财务区管理信息
description: 在项目财务区管理信息
author: Alina
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: d8c274d2153836647367c263cad8d786402cbe7f
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 2%

---

# 在项目财务区管理信息

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

您可以通过访问“项目详细信息”部分的“财务”区域来查看或编辑项目的财务信息。 在此区域中，可以查看或编辑的字段数量有限。 有关编辑项目所有信息的信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高程度地访问项目和财务数据</p> <p>编辑对项目和财务数据的访问权限以编辑项目的财务信息</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看包含查看财务权限的项目或更高版本的权限</p> <p>管理包含管理财务的项目的权限以编辑项目的财务信息</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 财务区域概述

在“财务”区域中查看或编辑信息时，请考虑以下事项：

* 您可以在“项目详细信息”的“财务”区域找到的财务信息表示从任务累计到项目层的值，以及直接在项目中输入的信息。 某些财务信息可以在项目和任务级别进行管理。
* 您必须拥有项目的查看权限以及从访问级别访问财务数据的权限，才能查看项目的财务区域。
* 您必须拥有项目的管理权限以及从访问级别访问财务数据的权限，才能编辑有关财务区域的信息。 但是，我们建议仅项目所有者应编辑此区域上的信息。

## 查看项目的财务信息

1. 转到项目。
1. 单击 **项目详细信息** 中。
1. 单击 **编辑** 图标 ![](assets/edit-icon.png) 在“详细信息”部分的右上角，单击 **金融**.

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >根据Workfront管理员配置布局模板的方式，概述部分可能不会最先列出，在这种情况下，该部分会折叠。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. 在项目的“财务”区域中查看以下字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">绩效指数方法</td> 
      <td> 控制Workfront用于计算“应得值”量度的方法。 它可以基于小时，也可以基于成本。 <br>有关PIM的更多信息，请参阅文章 <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">设置性能索引方法(PIM)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI / SPI / CSI</td> 
      <td> <p>这些是项目性能量度，用于显示您的项目在给定时间的执行情况。 这些值是根据性能指数方法计算的。<br>有关更多信息，请参阅以下文章： </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">计算成本绩效指数(CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">计算计划性能索引(SPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">计算成本计划绩效指数(CSI)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完工估算</td> 
      <td> 项目的预计总成本，如果绩效索引方法(PIM)基于小时，则以小时表示，如果绩效索引方法(PIM)基于成本，则以货币值表示。<br>有关在完成时计算估计的详细信息，请参阅文章 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">完成时计算估计(EAC)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">预算</td> 
      <td>这是项目的预算集。 这由项目所有者手动指定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">固定成本</td> 
      <td>这些是项目的固定成本，与项目的其他活动无关。 项目所有者手动输入这些值。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划成本</td> 
      <td>项目的估计成本，基于计划小时数和与任务分配人（职务角色或用户）关联的费率。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际成本</td> 
      <td>项目应计的所有成本。 实际成本是所有实际成本的总和：人工成本（基于实际工时和与职务职责或记录其用户关联的费率）、费用和固定成本（可与项目或任务关联）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">固定收入</td> 
      <td>根据项目计划设置预期收入。 固定收入由项目责任人手动指定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划收入</td> 
      <td>根据计划小时数和与任务分配人（职务角色或用户）关联的费率预计的预计收入。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际收入</td> 
      <td>根据实际工时和与任务分配人（职务职责或用户）关联的费率，从项目实际收入。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">已记帐收入</td> 
      <td> <p>已向客户或其他交易方开单的收入，这些收入在计费记录中被捕获。 有关帐单记录的更多信息，请参阅文章 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">创建帐单记录</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

## 编辑项目的财务信息

作为项目责任人，您可以编辑项目“财务”子选项卡上的信息。

要编辑“项目财务”子标签上的信息，请执行以下操作：

1. 转到您所有者的项目。

   >[!NOTE]
   >
   >您需要对项目的“管理”权限才能执行以下步骤。 我们还建议只有项目所有者才应更改项目的“财务”子选项卡。

1. 单击 **项目详细信息** 中。
1. 单击 **编辑** 图标 ![](assets/edit-icon.png) 在“详细信息”部分的右上角，单击 **金融** . 此时将打开“财务”区域进行编辑。
1. 通过单击字段或单击，编辑任何可编辑的字段 **+添加** 向空字段添加信息。

   >[!TIP]
   >
   >如果字段是由Workfront自动计算的，或者您没有这些字段的编辑权限，则这些字段将无法编辑。

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. 更新以下任意字段。

   >[!NOTE]
   >
   >根据Workfront管理员设置布局模板的方式，“项目详细信息”部分中的字段在您的环境中可能会有所不同。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">绩效指数方法</td> 
      <td> <p>控制Workfront用于计算项目绩效量度的方法。 这是由管理员在系统级别设置的，但您也可以在项目级别对其进行编辑。 请考虑选择以下选项之一：</p> 
       <ul> 
        <li><strong>基于小时：</strong>Workfront在计算项目的CPI和EAC时使用计划小时，项目的EAC显示为数字（以小时为单位）。 </li> 
        <li><strong>成本基础：</strong>Workfront在计算项目的CPI和EAC时使用计划人工成本，EAC显示为货币值。 选择此选项时，请确保任务分配人（职务角色或用户）与成本费率关联。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完工估算</td> 
      <td> <p>表示项目或任务完成时的预计总成本。 这是由管理员在系统级别设置的，但您也可以在项目级别对其进行编辑。 请考虑选择以下选项之一：</p> 
       <ul> 
        <li><strong>在项目级别计算</strong>:父任务和项目的EAC通过在EAC公式中输入实际工时/实际人工成本来确定。 此计算包括直接添加到父任务或项目的实际小时数/成本和费用。</li> 
        <li><strong>从任务/子任务汇总</strong>:父任务和项目的EAC通过汇总每个子任务的EAC来确定。 此计算不包括直接添加到父任务或项目的实际小时数/成本和费用。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">预算</td> 
      <td>指定此项目的预算。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">固定成本</td> 
      <td>指定此项目的固定成本。 这不应包括任何人工或费用成本。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">固定收入</td> 
      <td> <p>指定此项目的固定收入。 这不应包括来自向合作伙伴或第三方计费的任何账单记录的收入。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">项目货币</td> 
      <td> <p>如果此项目的货币与系统中的默认货币不同，请指定此项目的货币。 系统中的默认货币由Workfront管理员定义。 有关在Workfront中设置汇率的更多信息，请参阅文章 <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">设置汇率</a>.</p> </td> 
     </tr>
    </tbody> 
   </table>

1. 单击 **保存更改**.
