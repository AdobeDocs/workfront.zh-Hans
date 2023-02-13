---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 在Adobe Workfront中打印校样摘要
description: 您可以打印校样摘要、将其另存为PDF，或将其导出为针对Adobe Reader优化的XLS文件或PDF文件。
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 1%

---

# 在Adobe Workfront中打印校样摘要

您可以打印校样摘要、将其另存为PDF，或将其导出为针对Adobe Reader优化的XLS文件或PDF文件。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：选择或Premium</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（必须为用户启用校样）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校对权限配置文件 </td> 
   <td>经理或更高级别</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 打印校样摘要或将其另存为PDF文件

您可以直接从文档列表打印校样摘要。

>[!NOTE]
>
>您无法同时从文档列表打印多个校样摘要。

1. 在包含校样的文档列表中，将鼠标悬停在包含文档的行上，然后单击 **打印摘要**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   或

   在校样查看器中查看校样时，单击 **打印**&#x200B;图标 ![](assets/print-icon-in-pv.png) 中。 (如果左侧工具栏不可见，请单击“菜单”图标 ![](assets/menu-icon-in-pv.png) )。

1. 使用以下任意选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">显示</td> 
      <td> <p>指定要打印的内容：</p> 
       <ul> 
        <li>的 <strong>当前版本</strong> 或 <strong>所有版本</strong> 证据</li> 
        <li>仅 <strong>带有注释的页面</strong> 或 <strong>所有页面</strong></li> 
        <li>仅 <strong>页面缩略图</strong> （每个页面的小型渲染）或 <strong>完整页面</strong> （校样的完整呈现）<br></li> 
        <p>注意：要在打印输出中查看标记上的针脚数，您需要选择“完整页面”，而不是“页面缩览图”。 </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">评论排序依据</td> 
      <td> <p>（仅当您选择了上面的页面缩略图时才可用）指定希望打印校样注释的顺序：</p> 
       <ul> 
        <li><strong>Oldest</strong>:从首个评论到最后</li> 
        <li><strong>最新</strong>:从最后一次评论到第一次</li> 
        <li><strong>页面</strong>:按页面从第一页到最后一页，或从最后一页到第一页</li> 
        <li><strong>创建者</strong>:按添加了它们的用户名，从A-Z或Z-A</li> 
       </ul> <p>这些选项不会影响导出为XLS或PDF文件的输出。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">按</td> 
      <td> <p>您可以使用以下选项的任意组合在打印或导出为XLS或PDF文件的输出中仅包含某些注释：</p> 
       <ul> 
        <li>您选择的作者（默认）</li> 
        <li>您选择的操作</li> 
        <li><strong>未解决</strong> 状态</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作流</td> 
      <td> <p>（仅当校样具有自动工作流时可用）您可以单击 <strong>显示图</strong> 在打印输出中包含一个图表，其中显示了校样的阶段以及在每个阶段做出的决定。 在显示的图表中，颜色表示在舞台上做出的决策：</p> <p><strong>绿色</strong>:已批准</p> <p><strong>蓝色</strong>:等待决定</p> <p><strong>红色</strong>:所需决策的更改</p> <p><strong>灰色</strong>:尚未开始</p> <p><strong>黄色</strong>:已批准更改</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **打印**.
1. 在显示窗口的右侧面板中，如果要打印摘要，请单击 **目标** 菜单，然后单击 **查看更多**. 在显示的列表中单击要使用的打印机，然后单击 **打印**.

   或

   如果要将摘要另存为PDF文件，请单击 **目标** 菜单，单击 **另存为PDF**，然后单击 **保存**.

## 将校样摘要导出为XLS或PDF

您可以将静态内容的校样摘要导出为XLS文件或PDF文件。 校样导出仅包含校样的内容。

1. 在包含校样的文档列表中，将鼠标悬停在包含文档的行上，然后单击 **打印摘要**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. 单击页面右上角附近的XLS图标或PDF图标。

   ![](assets/xls-pdf-icons-350x136.png)

导出的文件准备就绪后，您会收到一封电子邮件，您可以从中下载文件。

如果将摘要导出为PDF文件，则校样上的注释会显示在PDF读取器中。 如果某个评论具有多个与其关联的标记，则该评论将多次显示在评论列表中（每个标记一次）。
