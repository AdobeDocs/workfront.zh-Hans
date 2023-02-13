---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: 计划自动报表提交
description: 计划自动报表提交
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 2%

---

# 计划自动报表提交

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

您可以安排报表按照定义的计划自动提交给用户，也可以一次性手动发送报表。 当您从Adobe Workfront发送报表时，用户将收到一封电子邮件，其中Workfront报表位于单独的附件中。

有关更多信息（包括可能影响报表交付的大小限制），请参阅 [报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

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
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须创建报表。 要了解有关创建报告的更多信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 计划报表提交

要计划报表自动提交或编辑或删除现有报表提交，请执行以下操&#x200B;作：

1. 转到要计划提交的报表。

   >[!NOTE]
   >
   >报表投放不包含提示。 如果您希望限制报表投放中的数据，我们建议将过滤器应用到您要发送的报表。

1. 单击 **报表操作**，则 **发送报表**.

   的 **发送报表** 对话框。

   >[!TIP]
   >
   >要在任何给定时间手动发送报表，请转到报表，然后单击 **报表操作** > **发送报表** > **立即发送**.

1. 选择 **重复投放** 选项卡。
1. （视情况而定）要修改现有的重复报表提交，请在 **重复投放** 中。
1. 指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>发送至</p> </td> 
      <td> <p>开始键入要将报表发送到的用户、群组、团队或角色的名称，然后在下拉列表中显示该名称时单击该名称。</p> <p>或</p> <p>指定您要访问报表的Workfront系统外部人员的电子邮件地址。</p> <p>重复此过程以将报表发送给多个用户、组、团队或角色。</p> <p>注释:  <p>添加报表提交收件人时，请考虑以下事项：</p> 
        <ul> 
         <li>如果贵组织将Workfront通知限制为特定的电子邮件域，则您可能只能将报表发送到电子邮件中列出的电子邮允许列表件地址。<p>有关Workfront管理员如何更新电子邮件允许列表的信息，请参阅部分 <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">配置电子邮件允许列表</a>.</p></li> 
         <li> <p>添加大量用户作为收件人可能会导致投放失败。 如果您遇到提交失败的情况，可以计划使用较小用户组进行多个报表提交。</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>电子邮件主题</p> </td> 
      <td> <p>指定电子邮件通知的主题。</p> <p>默认情况下，电子邮件的主题为：</p> <p><em>Workfront报告：[报表名称] [日期]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>电子邮件信息</p> </td> 
      <td> <p>指定要包含在电子邮件中的消息。</p> <p>默认情况下，电子邮件消息为：</p> <p><em>附件是Workfront在[日期]生成的[报表频度]报表[报表名称]。</em> </p> <p>注意：对于仅以Excel文件形式提交的报表，还会在电子邮件中添加以下消息：“请注意，使用MS Excel(XLS)文件类型时，这些文件类型支持的超链接数量存在限制(65,530)。 如果超出这些限制，您的文件将不会打开，建议在没有超链接的情况下重新发送。 请返回报表计划程序以删除超链接并重新发送报表。” “请返回到报表计划程序”短语是返回报表的链接。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>使用</p> </td> 
      <td> <p>开始键入有权访问报表的用户名称，然后在下拉列表中显示该名称时单击该名称。 接收报表的用户将获得与您在此处指定的用户相同级别的报表访问权限。<br> 有关更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">运行并提交具有其他用户访问权限的报表</a>.</p> <p>注意：此字段不支持通配符。 例如，使用通配符$User.ID时，不会使用接收报表的用户的访问权限来运行报表。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>格式</p> </td> 
      <td> <p>选择要用于已传送报表的格式：</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>如果选择此选项，则可以使用 <strong>纸张大小</strong> 和 <strong>方向</strong> 选项。</p> </li> 
        <li> <p>MS Excel(.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>包括链接</p> </td> 
      <td> <p>此选项仅在 <strong>MS Excel</strong> 的 <strong>格式</strong> 下拉菜单。 启用此选项后，导出的Excel文档中将包含所有超链接。</p> <p>无法打开包含65,530个以上链接的文档。 如果导出的文档将包含65,530个以上的链接，请取消选择此选项。</p> <p>默认情况下，此选项处于启用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>摘要</p> </td> 
      <td> <p>显示投放重复时间的摘要。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>重复</p> </td> 
      <td> <p>选择报表应按每日、每周、每月还是每年发送。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>重复，每当</p> </td> 
      <td> <p>选择您希望投放重复的频率。 为此选项选择的值基于 <strong>重复</strong> 下拉列表。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>时间</p> </td> 
      <td> <p>选择要发送投放的时间。</p> <p>提示：由于系统加载会影响报表提交时间，因此在计划时间与实际提交时间之间可能会存在延迟。 如果您需要按特定时间提交报表，我们建议在需要提交报表之前计划提交。 例如，我们建议在需要投放的日期之前的一天安排投放。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>重复，在</p> </td> 
      <td> <p>当 <strong>重复</strong> 选项设置为 <strong>每周</strong> 或 <strong>每月</strong>:</p> 
       <ul> 
        <li> <p>当 <strong>重复</strong> 选项设置为 <strong>每周</strong>:选择发送投放的一周中的天数。</p> </li> 
        <li> <p>当 <strong>重复</strong> 选项设置为 <strong>每月</strong>:选择投放是在月、周或月的最后一天发送(这些选项利用您在 <strong>开始时间</strong> 字段。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>开始时间</p> </td> 
      <td>选择计划提交的开始日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>结束日期</p> </td> 
      <td>选择计划提交的结束日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>从不</p> </td> 
      <td>选择 <strong>从不</strong> 如果您希望计划提交无限期地持续。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **保存** 以保存报表提交。

   报表显示在 **重复投放** 部分(在 **发送报表** 对话框)，并且它将在计划时间发送。

   有关可影响报表提交的大小限制的信息，请参阅 [报表提交限制](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) 和 [导出限制](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

1. （可选）要删除计划投放，请执行以下操作：

   1. 在 **重复投放** 面板，单击计划投放，然后单击 **删除**.
   1. 单击 **删除** 确认。

## 视频演示

观看以下视频，了解如何计划报表提交。 此视频在Workfront Classic中录制。 但是，该内容也适用于新的Workfront体验。

[ ![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Additional information</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See also:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Learning Path for reports and dashboards</a> </li>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/basic-report-creation-program">Basic Report Creation Program for the new Workfront experience</a> </p>
  -->
