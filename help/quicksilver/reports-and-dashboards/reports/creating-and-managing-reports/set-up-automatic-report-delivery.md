---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: 计划自动报表提交
description: 计划自动报表提交
author: Courtney
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: f78a86dcdf7b63e98bec5216fb5ab7622775a053
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 2%

---

# 计划自动报表提交

<!-- Audited: 4/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

您可以计划报表以按照定义的计划自动交付给用户，也可以手动一次性发送报表。 从Adobe Workfront发送报告时，用户会收到一封电子邮件，其中包含单独附件中的Workfront报告。

有关详细信息（包括可能影响报表交付的大小限制），请参阅[报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
      <td> 
      <p>新增：标准</p>
      <p>或</p>

<p>当前：计划</p>

</td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在开始之前，您必须创建一个报告。 要了解有关创建报告的详细信息，请参阅[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 计划报表提交


要计划报表的自动提交，请执行以下操作&#x200B;：

{{step1-to-reports}}

>[!NOTE]
>
>报告交付不包含提示。 如果您希望限制报告传送中的数据，我们建议您将过滤器应用于要发送的报告。

1. 在&#x200B;**报表**&#x200B;页面上，选择一个报表。
1. 在屏幕顶部，单击&#x200B;**报告操作**，然后从出现的下拉列表中&#x200B;**发送报告**。 显示&#x200B;**发送报告**&#x200B;对话框。

   >[!TIP]
   >
   >要在任何给定时间手动发送报告，请转到报告，然后单击&#x200B;**报告操作** > **发送报告** > **立即发送**。

1. 选择&#x200B;**重复传送**&#x200B;选项卡。
1. （视情况而定）要修改现有的重复报告传送，请在对话框右侧的&#x200B;**重复传送**&#x200B;部分中选择报告传送。
1. 指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>发送至</p> </td> 
      <td> <p>开始键入要向其发送报告的用户、组、团队或角色的名称，然后在名称出现在下拉列表中时单击该名称。</p> <p>或</p> <p>输入您希望有权访问报告的Workfront系统外部人员的电子邮件地址。</p> <p>重复此过程可将报告发送给多个用户、组、团队或角色。</p> <p>注意：  <p>添加报告投放收件人时，请考虑以下事项：</p> 
        <ul> 
         <li>如果贵组织将Workfront通知限制在特定电子邮件域，则您只能将报告发送到电子邮件允许列表中列出的电子邮件地址。<p>有关Workfront管理员如何更新电子邮件允许列表的信息，请参阅<a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">配置电子邮件允许列表</a>部分。</p></li> 
         <li> <p>添加大量用户作为收件人可能会导致投放失败。 如果您遇到交付失败的情况，则可以使用较小的用户组安排多个报表交付。</p> </li> 
        </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>电子邮件主题</p> </td> 
      <td> <p>输入电子邮件通知的主题。</p> <p>默认情况下，电子邮件主题为：</p> <p><em>Workfront报告： [报告名称] [日期]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>电子邮件信息</p> </td> 
      <td> <p>输入要包含在电子邮件中的消息。</p> <p>默认情况下，电子邮件消息为：</p> <p><em>附加是Workfront于[日期].</em>生成的[报告频率]报告[报告名称] </p> <p>注意：对于仅以Excel文件形式提供的报表，电子邮件中还会添加以下消息：“请注意，对于MS Excel (XLS)文件类型，这些文件类型支持的超链接数量存在限制(65,530)。 如果超过这些限制，文件将不会打开，建议在没有超链接的情况下重新发送。 请返回报告计划程序以删除超链接并重新发送报告。” “请返回到报告计划程序”短语是一个返回到报告的链接。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>提供此报告的访问权限：</p> </td> 
      <td> <p>开始键入有权访问报告的用户的名称，然后在名称出现在下拉列表中时单击该名称。 将授予接收报表的用户与您在此指定的用户相同级别的报表访问权限。<br>有关详细信息，请参阅<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">以其他用户的访问权限运行并交付报告</a>。</p> <p>注意：此字段不支持通配符。 例如，使用通配符<em>$$User.ID</em>不会通过接收报告的用户的访问权限运行报告。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>格式化</p> </td> 
      <td> <p>选择所传送报表的格式：</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>如果选择PDF，则可以使用显示的其他<strong>纸张大小</strong>和<strong>方向</strong>选项来格式化输出。</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>包括链接</p> </td> 
      <td> <p>仅当在<strong>格式</strong>下拉菜单中选择<strong>MS Excel</strong>时，此选项才可用。 启用此选项后，所有超链接都将包含在导出的Excel文档中。</p> <p>无法打开包含超过65,530个链接的文档。 如果导出的文档包含的链接超过65,530个，请取消选择此选项。</p> <p>此选项默认处于启用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>摘要</p> </td> 
      <td> <p>显示投放重复时间的摘要。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>重复</p> </td> 
      <td> <p>选择是否应每天、每周、每月或每年提交报表。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>重复，每当</p> </td> 
      <td> <p>选择您希望投放重复的频率。 您为此选项选择的值基于<strong>重复</strong>下拉列表中选择的选项。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>时间</p> </td> 
      <td> <p>选择一天中投放的发送时间。</p> <p>提示：由于系统加载可能会影响报表交付时间，因此计划时间与实际交付时间之间可能会有长达24小时的延迟。 如果您需要在特定时间之前提交报表，我们建议在所需时间之前安排提交。 通常，我们建议至少先在需要投放日期的前一天安排投放。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>重复，在</p> </td> 
      <td> <p>当<strong>重复</strong>选项设置为<strong>每周</strong>或<strong>每月</strong>时，此选项可用：</p> 
       <ul> 
        <li> <p>当<strong>重复</strong>选项设置为<strong>每周</strong>时：选择发送投放的每周日期。</p> </li> 
        <li> <p>当<strong>重复</strong>选项设置为<strong>每月</strong>时：选择发送投放的日期是当月的某一天、一周的某一天还是当月的最后一天（这些选项利用您在<strong>开始日期</strong>字段中选择的日期）。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>开始时间</p> </td> 
      <td>选择计划投放开始日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>结束日期</p> </td> 
      <td>选择计划投放结束的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>从不</p> </td> 
      <td>如果希望计划投放无限期地持续，请选择<strong>从不</strong>。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**&#x200B;以保存报告交付。 该报告显示在&#x200B;**发送报告**&#x200B;对话框的&#x200B;**重复传送**&#x200B;部分，将在计划时间发送。

   有关可能影响报表交付的大小限制的信息，请参阅[报表交付限制](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits)和[导出限制](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export)部分。

>[!IMPORTANT]
>
>处理计划报表以进行提交时，计划报表受内部时间限制。 如果报告发送时间超过限制，您将收到通知，并且无论剩余任何计划提交，都将不再提交报告。 要继续发送报告，首先尝试通过过滤器和视图减小报告的大小，然后创建新的计划提交。
>
>如果您使用计划报表交付通过BI工具分析Workfront数据，我们建议您改用Workfront Data Connect 。 有关详细信息，请参阅[Workfront Data Connect概述](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md)。

## 删除计划报表提交

要删除计划报表提交，请执行以下操作&#x200B;：

{{step1-to-reports}}

1. 在&#x200B;**报表**&#x200B;页面上，选择一个报表。

1. 在屏幕顶部，单击&#x200B;**报告操作**，然后从出现的下拉列表中&#x200B;**发送报告**。 显示&#x200B;**发送报告**&#x200B;对话框。

1. 选择&#x200B;**重复传送**&#x200B;选项卡。
1. 在对话框右侧的&#x200B;**重复传送**&#x200B;部分中，单击要删除的计划传送。
1. 在&#x200B;**重复传送**&#x200B;详细信息部分中，单击&#x200B;**删除**。

1. 单击&#x200B;**删除**&#x200B;以确认。

<!--## Video walk-through

View the following video to learn how to schedule a report delivery. This video was recorded in Workfront Classic. However, the content also applies to the new Workfront experience.

[ ![Video walkthrough of report delivery](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)


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
