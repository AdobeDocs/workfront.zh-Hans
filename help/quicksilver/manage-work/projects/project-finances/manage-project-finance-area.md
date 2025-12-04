---
product-area: projects
navigation-topic: financials
title: 管理项目财务领域的信息
description: 您可以通过访问项目详细信息部分的财务区域来查看或编辑项目的财务信息。
author: Lisa
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: f01ce9bcbb795097d39e276a734300f5059e35c4
workflow-type: tm+mt
source-wordcount: '1275'
ht-degree: 3%

---

# 管理项目财务方面的信息

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

您可以通过访问项目详细信息部分的财务区域来查看或编辑项目的财务信息。 您可以在此区域中查看或编辑的字段数量有限。 有关编辑项目的所有信息，请参阅[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td>
   <td>
   <p>浅色或更高</p>
   <p>审核或更高</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看或更高权限的项目和财务数据</p> <p>编辑对项目和财务数据的访问权限以编辑项目的财务信息</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看包含查看财务权限的项目或更高版本的权限</p> <p>管理包含管理财务的项目的权限以编辑项目的财务信息</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 财务领域概览

在财务区域查看或编辑信息时，请考虑以下事项：

* 您可以在“项目详细信息”的“财务”区域找到的财务信息表示从任务累计到项目层的值，以及直接在项目中输入的信息。 有些财务信息可以在项目级别和任务级别进行管理。
* 您必须具有项目的“查看”权限以及从访问级别访问“财务数据”，才能查看项目的财务区域。
* 您必须具有项目的管理权限以及从访问级别访问财务数据，才能编辑财务区域上的信息。 但是，我们建议仅项目所有者编辑此区域上的信息。

## 查看项目的财务信息

1. 转到项目。
1. 单击左侧面板中的&#x200B;**项目详细信息**。
1. 单击“详细信息”部分右上角的&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)，然后单击&#x200B;**财务**。

   ![详细资料视图中的财务区域](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >根据Workfront管理员配置布局模板的方式，概述部分可能不会列在首位，在这种情况下，它会折叠。 有关信息，请参阅[使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

1. 在项目的财务区域查看以下字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">绩效指数方法</td> 
      <td> 控制Workfront用于计算“实现值”指标的方法。 它可以基于小时数，也可以基于成本。 <br>有关PIM的详细信息，请参阅文章<a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">设置绩效指数方法(PIM)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI/SPI/CSI</td> 
      <td> <p>这些项目绩效指标可显示项目在给定时间的执行情况。 其值根据绩效指数法计算。<br>有关详细信息，请参阅以下文章： </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">计算成本绩效指数(CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">计算计划绩效指数(SPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">计算成本计划绩效指数(CSI)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完工估算</td> 
      <td> 项目的预计总成本，如果绩效指数方法(PIM)基于小时，则以小时表示；如果绩效指数方法(PIM)基于成本，则以货币值表示。<br>有关计算完工估算的详细信息，请参阅文章<a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">计算完工估算(EAC)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">预算</td> 
      <td>这是为项目设置的预算。 这由项目所有者手动指定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">固定成本</td> 
      <td>这些是项目的固定成本，与项目上的其他活动无关。 它们由项目所有者手动输入。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">规划成本</td> 
      <td>项目的估计成本，基于计划小时数以及与任务受让人（工作角色或用户）关联的费率。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际成本</td> 
      <td>项目的所有应计成本。 实际成本是所有实际成本的总和：人工成本（基于实际小时数以及与工作角色或记录工作角色的用户关联的费率）、费用和固定成本（可与项目或任务关联）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">固定收入</td> 
      <td>设置基于项目计划的预期收入。 固定收入由项目所有者手动指定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">规划收入</td> 
      <td>基于计划小时数和与任务受让人（工作角色或用户）关联的费率的预计收入。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际收入</td> 
      <td>基于实际小时数和与任务受让人（职位角色或用户）关联的费率的项目实际收入。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">已记帐收入</td> 
      <td> <p>向客户或其他方记帐的收入，这些收入记录在帐单记录中。 有关开票记录的详细信息，请参阅文章<a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">创建开票记录</a>。 </p> </td> 
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

作为项目所有者，您可以编辑项目的财务子选项卡上的信息。

要编辑“项目财务”子标签上的信息，请执行以下操作：

1. 转到您拥有的项目。

   >[!NOTE]
   >
   >您需要具有项目管理权限才能执行以下步骤。 我们还建议仅项目所有者应对项目的财务子选项卡进行更改。

1. 单击左侧面板中的&#x200B;**项目详细信息**。
1. 单击“详细信息”部分右上角的&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)，然后单击&#x200B;**财务**。 这将打开“财务”区域以进行编辑。
1. 编辑任何可编辑的字段，方法是单击该字段或单击&#x200B;**+添加**&#x200B;将信息添加到空字段。

   >[!TIP]
   >
   >如果字段由Workfront自动计算或您没有编辑权限，则无法对其进行编辑。

   ![编辑财务区域](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. 更新以下任意字段。

   >[!NOTE]
   >
   >根据Workfront管理员如何设置布局模板，您的环境中，项目详细信息部分中的字段可能不同。 有关信息，请参阅[使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">绩效指数方法</td> 
      <td> <p>控制Workfront用于计算项目绩效指标的方法。 此操作由管理员在系统级别设置，但您也可以在项目级别进行编辑。 请考虑选择以下选项之一：</p> 
       <ul> 
        <li>基于<strong>小时：</strong>Workfront在计算项目的CPI和EAC时使用计划小时数，并且项目的EAC显示为小时数。 </li> 
        <li><strong>基于成本：</strong>Workfront在计算项目的CPI和EAC时使用计划劳力成本，并且EAC显示为货币值。 选择此选项时，请确保您的任务受分配人（职位角色或用户）与成本费率相关联。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完工估算</td> 
      <td> <p>表示项目或任务完成时的预计总成本。 此操作由管理员在系统级别设置，但您也可以在项目级别进行编辑。 请考虑选择以下选项之一：</p> 
       <ul> 
        <li><strong>在项目级别计算</strong>：在EAC公式中输入实际小时数/实际劳力成本来确定父任务和项目的EAC。 此计算包括直接添加到父任务或项目的实际小时数/成本和费用。</li> 
        <li><strong>从任务/子任务汇总</strong>：父任务和项目的EAC通过汇总每个子任务的EAC来确定。 此计算不包括直接添加到父任务或项目的实际小时数/成本和费用。</li> 
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
      <td> <p>指定此项目的固定收入。 这不应包括来自向合作伙伴或第三方计费的任何计费记录的收入。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">项目货币</td> 
      <td> <p>如果此项目不同于系统中的默认货币，请指定该项目的货币。 系统中的默认货币由Workfront管理员定义。 有关在Workfront中设置汇率的更多信息，请参阅文章<a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">设置汇率</a>。</p> </td> 
     </tr>
    </tbody> 
   </table>

1. 单击&#x200B;**保存更改**。
