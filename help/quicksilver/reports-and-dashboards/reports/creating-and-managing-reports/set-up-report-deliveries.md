---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: 报表交付概述
description: 报表交付概述
author: Nolan
feature: Reports and Dashboards
exl-id: 1637df59-ca1d-4cf6-b83d-2b27936cdb96
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1528'
ht-degree: 0%

---

# 报表交付概述

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is linked to the UI in the Send Report box inside the Preview sandbox. If you change title, log bug for Dev to fix the link) </p>
-->

您可以安排报表按照定义的计划自动提交给用户，也可以手动一次性发送报表。 当您从Adobe Workfront发送报表时，用户将收到一封电子邮件，其中Workfront报表位于单独的附件中。

有关设置报表以进行提交的信息，请参阅文章 [计划自动报表提交](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

您既无法计划报表的提交，也无法在预览沙盒环境中手动提交报表。 有关预览沙盒的更多信息，请参阅文章 [Adobe Workfront预览沙盒环境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).\
有关在预览沙盒环境中传送报表的更多信息，请参阅文章 [在预览沙盒环境中发送报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/send-report-preview-sandbox-environment.md).

## 报表提交限制

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."])</p>
-->

在计划报表提交时，请考虑以下事项：

* 您最多可以为任何给定报表安排10个重复报表提交。
* 您只有在创建报表时才能安排提交报表。 如果您需要发送未创建的报表，则可以手动发送。

## 导出限制

存在一些大小限制，这些限制会影响报表在Workfront中的显示方式，以及它们通过手动导出、提交报表或API导出的方式：

* **5MB文件大小：** 计划提交的任何导出报表的文件大小限制。 如果附加到电子邮件的导出文件大于5MB，则会通过电子邮件发送可下载文件的链接，而不是附加的导出报表。 

   >[!NOTE]
   >
   >大于5MB的Excel .xlsx文件不会生成电子邮件。 您可以手动将报表导出为此格式。 有关导出报表的信息，请参阅 [导出数据](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* **50,000行：** .pdf和制表符分隔文件的报表导出中允许的数据行数。

   对于Excel .xls文件，此限制为 **65,000行**.

   对于Excel .xlsx文件，此限制为 **10万行**.

   这些限制不包括列标题以及报表中分组的行。 例如，如果您在一个报表中有6个分组，并且有50,000行或数据，则导出的文件将有50,000行。

   如果报表的项目数超过这些限制，则会收到一个错误，指出导出和提交报表失败。 将屏幕上显示的项目数量减少到小于或等于这些限制的数量，以便能够交付结果。 如果要导出所有数据，我们建议您使用过滤器获取较小数据负载，然后执行多次导出。 有关更多信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

   这些限制适用于：

   * 手动导出报表。
   * 计划报表。
   * 通过API集成导出。 
   * 通过启动导出的数据。

      有关通过启动导出数据的更多信息，请参阅文章 [通过Kick-Starts从Adobe Workfront导出数据](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

      >[!NOTE]
      在启动文件中可导出50,000行，但只能导出为Excel格式文件。 

   * 导出项目的利用率信息。

      有关导出项目利用率信息的更多信息，请参阅 [资源利用率报告概述](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* **65,530个超链接：** 这是Excel对包含65,530个以上超链接的文档所施加的限制。 这些文档在手动导出或在提交的报表中发送时无法打开。 请注意，Excel文档可能只有200行数据，但如果文档内有超过65,530个链接，则该文档不会打开。 此限制仅存在于Excel文件中，而不存在于其他支持的格式中。 
* **256列**：这是Excel对包含256列以上的文档所施加的限制。 这些文档无法手动导出，也无法在提交的报表中发送。 此限制仅存在于Excel文件中，而不存在于其他支持的格式中。 

如果尝试导出超出限制的数据，您可能不会在导出中收到所有预期数据。 而是在限制内生成修改的报告。 

此外，运行时间超过60分钟的报表将被停止。

如果您对限制有任何疑问或疑问，请联系Workfront技术支持。

## 了解已传送报表上的时间戳

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Note about if this is delivered at a time based on the user's time zone settings?)</p>
-->

当您通过电子邮件接收报表时，如果要在Workfront中同时查看报表，则报表的时间戳和时间格式可能与Workfront中的时间戳和时间格式不匹配。 

请考虑以下事项： 

* 在浏览器中查看报表时，报表上的时间戳和格式与浏览器的区域设置和时区（在浏览器设置中定义）匹配。
* 在电子邮件中提交报表时，报表会随时间戳和格式一起提交，这些时间戳和格式与Workfront配置文件中指定的用户区域设置和时区相匹配。\
   有关Workfront中用户区域设置和时区的更多信息，请参阅文章 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 具有特殊视图的报表 {#reports-with-a-special-view}

将特殊视图应用于报表时，该特殊视图会显示在Workfront报表的“详细信息”选项卡中。

计划发送具有特殊视图的报表时，默认的“详细信息”选项卡会在已发送电子邮件的附件中发送，而不是在特殊视图中发送。

以下是一些特殊意见：

* 项目报表中的里程碑视图
* 项目或任务报表上的甘特图视图
* 以图表作为默认选项卡的报表

>[!NOTE]
除了具有特殊视图的默认选项卡外，如果报表上还有一个“矩阵”选项卡，则报表会像在“矩阵”选项卡上显示一样进行提交。

有关如何对报表应用特殊视图的详细信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 使用提交的文件

 当您从Workfront发送报表时，用户会收到一封电子邮件，其中报表位于单独的附件中。 

* [主题行、附件名称和报表标题](#subject-line-attachment-name-and-report-title)
* [时间戳](#timestamps)
* [品牌化](#branding)
* [格式](#formatting)
* [链接](#links)

### 主题行、附件名称和报表标题 {#subject-line-attachment-name-and-report-title}

有关已投放报表电子邮件主题行的更多信息，请参阅 [计划自动报表提交](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

所附报告的名称为： *The_Name_Of_The_Report*&#x200B;后跟导出的文件格式。 

如果您计划将提交的报表格式设置为PDF或HTML文件，则报表的标题将为：

*报表的名称。*

计划以Excel、Excel(.xlsx)或TSV格式提交的报表没有标题。

>[!NOTE]
如果报表包含描述，则该描述将包含在导出的文件中(如果文件的格式为PDF或HTML文件)。

### 时间戳 {#timestamps}

仅当文件格式为.pdf时，才会在附加的文件上显示时间戳。 时间戳位于附加文件的页脚中。

时间戳包括：

* 日期
* 时间
* 发送报表时区

### 品牌化 {#branding}

如果您的Workfront管理员已向Workfront实例添加了自定义品牌，则以.pdf格式发送的报表也将包含您的个性化徽标。

以所有其他格式发送的报表无法使用您的徽标进行个性化。

有关品牌化Workfront实例的更多信息，请参阅文章 [品牌化Adobe Workfront实例](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### 格式 {#formatting}

在发送或计划发送报表以进行提交时，您始终会收到报表的默认选项卡，除非报表具有特殊视图。

如果您的报表在Web应用程序中具有特殊格式，则当仅为.pdf和Excel文件交付详细信息和矩阵选项卡时，报表应使用特殊格式交付。

报表的过滤器、视图或分组不会包含在提交的文件中。 仅当您将报表作为PDF文件发送时，才会包含报表的描述。

有关接收具有特殊视图的报表的更多信息，请参阅文章 [具有特殊视图的报表](#reports-with-a-special-view).\
有关选择报表默认选项卡和特殊格式的详细信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### 链接 {#links}

将报表从Workfront发送到Excel或Excel格式时，原始文档中存在的任何工作链接将保留在已发送文件中。 链接可以指向Workfront中支持链接的任何对象。

电子邮件中报表的名称也是一个链接。

## 计划报表报告

您可以通过创建以下内容来查看报表是否已配置为提交：

* **视图** 对于列表或报表报表中的报表对象：在报表列表或报表报表报表中创建视图，并将以下列添加到视图：\
   *计划报表名称。\
   *为该报表计划的所有投放的名称都会列在项目符号列表的列中。\
   ![scheduled_reports_info_in_view_png](assets/scheduled-reports-info-in-view-350x294.png)

* **过滤器** 对于报表对象：在报表列表或报告报表中创建过滤器，并使用以下语句： *计划报表ID不为空*.\
   这将仅显示已在您的列表或报表中计划的报表。\
   ![](assets/qs-scheduled-report-filter-350x101.png)\
   有关创建报表的更多信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). 有关创建报告的信息，请参阅 [创建报告活动报告](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Scheduling a Repeating&nbsp;Report Delivery</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can schedule up to 10 repeating report deliveries for any given report.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can schedule a report to be delivered only if you are the creator of the report. If you need to send a report that you did not create, you can send it on a manual basis.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To schedule&nbsp;a report for automatic delivery or to edit an existing report delivery:&nbsp;​</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report for which you want to schedule delivery.&nbsp;</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The <strong>Send Report</strong> dialog box is displayed.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the <strong>Repeating Deliveries</strong>&nbsp;tab.<br><img src="assets/report-delivery-schedule-350x169.png" alt="" style="width: 350;height: 169;"></li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Conditional)&nbsp;To modify an existing repeating report delivery, select the report delivery in the <strong>Repeating Deliveries</strong>&nbsp;section.</li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Specify the following information:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Send to:</strong> Begin typing the name of the user, group, team, or role who you want to send&nbsp;the report to, then click the name when it appears in the drop-down list.<br>Or<br>Specify the email address of a person external to the Workfront system who you want to have access to the report.<br> Repeat this process to send the report to multiple users, groups, teams, or roles.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Subject:</strong> Specify a subject for the email notification.<br> By default, the email subject is: <em>Workfront Report: <Name of the report> Date of the Export</em>.<strong></strong></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Message:</strong> Specify a message to include in the email.<br>By default, the email message is:&nbsp;<em>Attached is the <report frequency> report <Name of the report> generated by Workfront on <Date>.</em><br>
   <note type="note">
   For reports delivered as an Excel file only, the following message is also added to the email: "Please be aware that with MS Excel (XLS) file types, there is a limit (65,530) on the number of hyperlinks these file types support. If you exceed those limits, your file will not open and it is recommended to resend without the hyperlinks.&nbsp;Please go back to the report scheduler&nbsp;to remove hyperlinks and resend the report." The "please go back to the report scheduler" phrase is a link back to the report.&nbsp;
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Deliver this report with the Access Rights of:</strong>&nbsp;Begin typing the name of a user who has access to the report, then click the name when it appears&nbsp;in the drop-down list. Users who receive the report will be granted the same level of access to the report as the user that you specify&nbsp;here.<br> For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>
   <note type="note">
   This field does not support wildcards. For example, using the wildcard $$User.ID does not run the report with the access rights of the user who is receiving the report.
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Format:</strong> Select in which of the following formats you want the report to be delivered:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> HTML</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">PDF</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS&nbsp;Excel</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS Excel (.xlsx)</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">TSV &nbsp;</li>
   </ul></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Include Links:</strong>&nbsp;This option is available&nbsp;only when <strong>MS Excel</strong> is selected in the <strong>Format</strong> drop-down menu. When this option is enabled, any hyperlinks are included in the exported Excel document. <br>Documents that contain more than 65,530 links cannot be opened. If the exported document will contain more than 65,530 links, deselect this option.<br>This option is enabled by default.&nbsp;</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Summary:</strong> Displays a summary of when the delivery repeats.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats:</strong> Select whether the report should be delivered daily, weekly, monthly, or yearly.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats Every:</strong> Select the frequency with which you want&nbsp;the delivery to repeat. The value you select for this option is&nbsp;based on the option that is selected in the <strong>Repeats</strong>&nbsp;drop-down list.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Time:</strong> Select the time of day for the delivery to be sent.</li>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats On:</strong>&nbsp;This option is available when the <strong>Repeats</strong>&nbsp;option is set to either <strong>Weekly</strong>&nbsp;or <strong>Monthly</strong>.</p>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the <strong>Repeats</strong>&nbsp;option is set to <strong>Weekly</strong>: Select the days of the week that the delivery is sent.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the <strong>Repeats</strong>&nbsp;option is set to <strong>Monthly</strong>: Select whether the delivery is sent on the day of the month, day of the week, or last day of the month (these options leverage the date that you select in the <strong>Starts On</strong>&nbsp;field).</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Starts On:</strong> Select the date for the scheduled delivery to begin.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Ends On:</strong> Select a date for the scheduled delivery to end. <br>Or</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Never</strong>&nbsp;if you want the scheduled delivery to last indefinitely.</li>
   -->

<!--
   <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save</strong>&nbsp;to save the report delivery.<br> The report is saved in the <strong>Repeating Deliveries</strong>&nbsp;section&nbsp;(in the <strong>Send Report</strong> dialog box).<br> The report will be sent at the schedule time<br>Or<br>To manually send the report, click <strong>Send Now</strong>.<br>For more information about sending the report instantly or manually, see&nbsp;.</li>
   -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a Scheduled Report Delivery</h2>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to the report with the delivery you want to delete.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then <strong>Send Report</strong>.&nbsp;</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Repeating Deliveries</strong>.&nbsp;</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the name of the scheduled delivery you want to delete, then click <strong>Delete</strong>. The report is no longer set up for the scheduled delivery.&nbsp;</li>
   -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Sending a Report Manually, on a One-Time Basis</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can manually send a report&nbsp;that has been previously scheduled, or you can create a single-use report delivery.​</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a title="Setting Up Report Deliveries" href="#sending-a-scheduled-report-now" class="MCXref xref">Sending a Scheduled Report Now</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a title="Setting Up Report Deliveries" href="#sending-a-report-one-time-only" class="MCXref xref">Sending a Report (One Time Only)</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="sending-a-scheduled-report-now">Sending a Scheduled Report Now</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">After a scheduled report has been set up, you can manually send the report rather than&nbsp;waiting until the scheduled time.</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report that you want to send now.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The Send Report dialog box is displayed.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>Repeating Deliveries</strong> tab.</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Repeating Deliveries</strong>&nbsp;section, select the report delivery that was previously created.<br><img src="assets/report-delivery-schedule-send-350x160.png" alt="" style="width: 350;height: 160;"></li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Send Now</strong>.<br> The report is sent to all users identified in the scheduled delivery.</li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="sending-a-report-one-time-only">Sending a Report (One Time Only)</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can manually send a report at any time. When you send a report in this way, delivery information (such as&nbsp;the users you are sending to and&nbsp;the email subject) are not saved. If you want to create a report delivery that you can save for later use, create a repeating scheduled report.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To send a report to users (one time only):</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report that you want to send now.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The <strong>Send Report</strong> dialog box is displayed.<br><img src="assets/report-delivery-sendnow-350x351.png" alt="" style="width: 350;height: 351;"></li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">On the <strong>Send Now</strong>&nbsp;tab, specify the following information:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Send to:</strong> Begin typing the name of the user, group, team, or role who you want to send&nbsp;the report to, then click the name when it appears in the drop-down list.&nbsp;Or, specify the email address of a person external to the Workfront system who you want to have access to the report.<br> Repeat this process to send the report to multiple users, groups, teams, or roles.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Subject:</strong> Specify a subject for the email notification.<br> By default, the email subject is: <em>Workfront Report: <Name of the report> Date of the Export</em>.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Message:</strong> Specify a message to include in the email.<br>By default, the email message is:&nbsp;<em>Attached is the <report frequency> report <Name of the report> generated by Workfront on <Date>.</em><br>
   <note type="note">
   For reports delivered as an Excel file only, the following message is also added to the email: "Please be aware that with MS Excel (XLS) file types, there is a limit (65,530) on the number of hyperlinks these file types support. If you exceed those limits, your file will not open and it is recommended to resend without the hyperlinks.&nbsp;Please go back to the report scheduler&nbsp;to remove hyperlinks and resend the report." The "please go back to the report scheduler" phrase is a link back to the report.&nbsp;
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Deliver this report with the Access Rights of:</strong>&nbsp;Begin typing the name of a user who has access to the report, then click the name when it appears&nbsp;in the drop-down list. Users who receive the report will be granted the same level of access to the report as the user that you specify&nbsp;here.<br> For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>.
   <note type="note">
   This field does not support wildcards. For example, using the wildcard $$User.ID does not run the report with the access rights of the user who is receiving the report.
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Format:</strong> Select in which of the following formats you want the report to be delivered:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> HTML</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">PDF</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS Excel</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS&nbsp;Excel (.xlsx)</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">TSV</li>
   </ul></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Include Links:</strong>&nbsp;This option is available&nbsp;only when <strong>MS Excel</strong> is selected in the <strong>Format</strong> drop-down menu. When this option is enabled, any hyperlinks are included in the exported Excel document. <br>Documents that contain more than 65,000 links cannot be opened. If the exported document will contain more than 65,000 links, deselect this option.<br>This option is enabled by default.</li>
   </ul></li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Send Now</strong>.<br> The report is sent to all users that you identified.<br> Or<br> Click <strong>Make Repeating Delivery</strong>&nbsp;if you want to set up&nbsp;a scheduled delivery with this same information, then complete the additional information regarding the frequency of when the report is sent.</li>
   -->
