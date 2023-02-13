---
user-type: administrator
product-area: system-administration
keywords: kickstart，kickstart，kickstarts，kickstarts
navigation-topic: use-kick-starts
title: 通过Kick-Starts从Adobe Workfront导出数据
description: 作为Adobe Workfront管理员，您可以使用Kick-Starts数据导出程序从Workfront导出数据。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1101'
ht-degree: 9%

---

# 通过Kick-Starts从Adobe Workfront导出数据

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

作为Adobe Workfront管理员，您可以使用Kick-Starts数据导出程序从Workfront导出数据。 在导出后，您可以在其他应用程序中使用它。

通过Kick-Start导出数据还有助于了解哪些字段与每个对象关联，这些字段的编码方式，以及这些字段的值在数据库中的格式。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用启动导出数据的利弊

在Workfront中可以通过两种方式导出数据：

* 从报表或列表导出数据

   有关从报表或列表导出数据的更多信息，请参阅 [导出数据](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* 通过启动导出数据

下表显示了每种方法的优缺点：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>导出的数据包括对象和字段值</p> </th> 
   <th> <p>能够同时导出多个对象类型周围的数据</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>从列表视图导出数据</strong> </p> <p>有关从列表导出数据的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">导出数据</a></p> </td> 
   <td> <p>是</p> <p>将导出与对象关联的Workfront本机字段和自定义字段。</p> </td> 
   <td> <p>否</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>通过Kick-Start导出数据</strong> </p> </td> 
   <td> <p>是（有限）</p> <p>与对象关联的大多数Workfront本机字段都会导出，但有些字段则不会导出。 例如，您无法通过项目启动导出导出来导出“计划”、“项目所有者”或“项目赞助商”字段。</p> <p>在附加了自定义表单的项目中，不会导出在表单的字段中输入的任何数据。</p> <p>但您可以导出自定义表单。 生成的文件列出了表单中配置的字段，如文本框和单选按钮。</p> </td> 
   <td> <p>是</p> <p>使用Kick-Starts导出Workfront数据，您可以在一次导出中导出与多个对象类型相关的数据。 例如，您可以在单次导出中包含任务、问题和项目。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 导出限制

通过启动导出数据时（数据以Excel文件格式导出）存在以下限制：

* **50,000行：** 文件中允许的行数。
* **65,530个超链接：** 这是Excel对包含65,530个以上超链接的文档所施加的限制。 这些文档在导出后无法打开。 请注意，Excel文档可能只有200行数据，但如果文档内有超过65,530个链接，则该文档不会打开。

## 通过启动导出数据

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统** > **开球，** 然后单击 **导出数据。**

1. 选择要导出的对象。
1. 单击 **更多选项** 查看对象的完整列表。

   此处列出的所有对象也可用于将数据导入Workfront。

   唯一的例外是 **访问级别** 对象。 导出中包含的访问级别数据表仅供参考。 它允许您按ID为新用户帐户分配访问级别。

   有关通过启动将数据导入Workfront的更多信息，请参阅 [使用“启动”模板将数据导入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). 以下是可通过启动导出的所有对象的列表：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>对象</p> </th> 
      <th> <p>Excel文件的导出工作表</p> </th> 
      <th> <p>导出格式</p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top">访问级别</td> 
      <td scope="col" valign="top">访问级别<br>首选项</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">分配</td> 
      <td scope="col" valign="top">分配<br>首选项</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">公司</td> 
      <td scope="col" valign="top"> 公司<br>首选项 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">电子邮件模板</td> 
      <td scope="col" valign="top"> 电子邮件模板<br>首选项 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">费用</td> 
      <td valign="top"> 费用<br>首选项 </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">外部页面</td> 
      <td valign="top"> 外部页面<br>首选项 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">筛选</td> 
      <td valign="top"> 过滤器<br>首选项 </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">组</td> 
      <td valign="top"> 组<br>首选项  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">分组</td> 
      <td valign="top"> 分组<br>首选项 </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">小时</td> 
      <td valign="top"> 小时<br>首选项 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">问题</td> 
      <td valign="top"> 问题<br>首选项 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">工作角色</td> 
      <td valign="top"> 作业角色<br>首选项 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">里程碑路径</td> 
      <td valign="top"> 里程碑<br>里程碑路径<br>首选项 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">注释</td> 
      <td valign="top"> 注意<br>首选项 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">项目组合</td> 
      <td valign="top"> Portfolio<br>首选项  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">项目</td> 
      <td valign="top"> 队列<br>项目<br>路由规则<br>队列主题<br>首选项 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">资源评估</td> 
      <td valign="top"> 资源估计<br>首选项 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">资源池</td> 
      <td valign="top"> 资源池<br>首选项 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">风险</td> 
      <td valign="top"> 风险<br>首选项  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">风险类型</td> 
      <td valign="top"> 风险类型<br>首选项  </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">记分卡</td> 
      <td valign="top">记分卡问题<br>记分卡选项<br>记分卡<br>首选项 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">任务</td> 
      <td valign="top"> 任务<br>首选项 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">模板</td> 
      <td valign="top"> 队列<br>模板<br>路由规则<br>队列主题<br>首选项 </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">模板分派</td> 
      <td valign="top"> 模板分配<br>首选项 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">模板任务</td> 
      <td valign="top"> 模板任务<br>首选项 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">时间表</td> 
      <td valign="top"> 时间表配置文件<br>时间表<br>首选项 </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> 查看 </td> 
      <td valign="top"> 查看<br>首选项  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **下载。**

   导出的启动文件将作为Excel文件或下载到计算机。 包含多个Excel和属性文件的zip文件。 每个Excel文件都是工作表的集合，其中每个工作表都表示与所选对象关联的字段。 有 **属性** 与每个导出关联的工作表。

   的 **功能板** 和 **报表** 选项允许您选择要包含在下载中的特定功能板和报表。 您只能导出在系统范围内共享的功能板。

   无法导出矩阵报表。 有关矩阵报表的更多信息，请参阅 [创建矩阵报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   在一次导出中，您最多可以选择100个功能板和100个报表。

   ![](assets/kickstart-export-350x381.png)

   一次可导出多个对象。

   默认情况下，以下对象显示在 **要包含的内容** 标签(在单击 **更多选项**):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>对象</strong> </p> </th> 
      <th> <p><strong>Excel文件的导出工作表</strong> </p> </th> 
      <th> <p> <strong>导出格式</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>仪表板</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>参数<br>参数选项<br>参数组<br>类别参数<br>类别<br>报表<br>“门户”选项卡部分<br>功能板<br>首选项</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>报告</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">参数<br>参数选项<br>参数组<br>类别参数<br>类别<br>报表<br>首选项</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>审批</p> </td> 
      <td scope="col" valign="top"> <p>步骤审批者<br>批准步骤<br>批准<br>审批流程<br>首选项</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>自定义数据</p> </td> 
      <td scope="col" valign="top"> <p>参数<br>参数选项<br>参数组<br>类别参数<br>类别<br>首选项</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>费用类型</p> </td> 
      <td valign="top"> <p>费用类型<br>首选项</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>小时数类型</p> </td> 
      <td valign="top"> <p>小时类型<br>首选项</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>团队</p> </td> 
      <td valign="top"> 团队成员<br>团队<br>首选项 </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>用户</p> </td> 
      <td valign="top"> <p>用户<br>首选项</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong></strong> </p> </th> 
      <th> <p><strong>Excel文件的导出工作表</strong> </p> </th> 
      <th> <p> <strong>导出格式</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>仪表板</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>参数<br>参数选项<br>参数组<br>类别参数<br>类别<br>报表<br>“门户”选项卡部分<br>功能板<br>首选项</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>报告</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">参数<br>参数选项<br>参数组<br>类别参数<br>类别<br>报表<br>首选项</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>审批</p> </td> 
      <td scope="col" valign="top"> <p>步骤审批者<br>批准步骤<br>批准<br>审批流程<br>首选项</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>自定义数据</p> </td> 
      <td scope="col" valign="top"> <p>参数<br>参数选项<br>参数组<br>类别参数<br>类别<br>首选项</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>费用类型</p> </td> 
      <td valign="top"> <p>费用类型<br>首选项</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>小时数类型</p> </td> 
      <td valign="top"> <p>小时类型<br>首选项</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>团队</p> </td> 
      <td valign="top"> 团队成员<br>团队<br>首选项 </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>用户</p> </td> 
      <td valign="top"> <p>用户<br>首选项</p> </td> 
      <td valign="top"> <p>Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （推荐）分析导出的数据，以确保导出您希望看到的所有信息。

   对于大型导出，Workfront会在后台工作以生成Excel文件，并会向您显示延迟警告消息。 启动文件会在下载完成后通过电子邮件发送给您。

   ![](assets/large-kick-start-file-warning-350x65.png)
