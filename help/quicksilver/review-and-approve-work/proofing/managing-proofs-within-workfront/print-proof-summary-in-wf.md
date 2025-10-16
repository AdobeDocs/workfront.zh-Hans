---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 在Adobe Workfront中打印验证摘要
description: 您可以打印验证摘要，将其另存为PDF，或导出为针对Adobe Reader优化的XLS文件或PDF文件。
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 1%

---

# 在Adobe Workfront中打印验证摘要

您可以打印验证摘要，将其另存为PDF，或导出为针对Adobe Reader优化的XLS文件或PDF文件。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>标准</p>
   <p>工作或计划</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 打印验证摘要或将其另存为PDF文件

您可以直接从文档列表打印验证摘要。

>[!NOTE]
>
>* 不支持大于1 GB的摘要。
>* 您无法同时打印文档列表中的多个校对摘要。

1. 在包含验证的文档列表中，将鼠标悬停在包含该文档的行上，然后单击&#x200B;**打印摘要**。

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   或

   在验证查看器中查看验证时，单击左侧工具栏中的&#x200B;**打印**&#x200B;图标![打印图标](assets/print-icon-in-pv.png)。 （如果左侧工具栏不可见，请单击验证查看器左上角的菜单图标![菜单图标](assets/menu-icon-in-pv.png)。）

1. 使用以下任一选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">显示</td> 
      <td> <p>指定要打印的内容：</p> 
       <ul> 
        <li>验证的<strong>当前版本</strong>或<strong>所有版本</strong></li> 
        <li>仅包含评论的<strong>页面</strong>或<strong>所有页面</strong></li> 
        <li>仅<strong>页面缩略图</strong>（每个页面的小量渲染）或<strong>完整页面</strong>（验证的完整渲染）<br></li> 
        <p>注：要在打印输出中查看标记上的固定编号，您需要选择“整页”，而不是“页面缩略图”。 </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">评论排序方式</td> 
      <td> <p>（仅在上面选择页面缩略图时可用）指定校样注释的打印顺序：</p> 
       <ul> 
        <li><strong>Oldest</strong>：从第一个评论到最后一个</li> 
        <li><strong>Latest</strong>：从上一个评论到第一个评论</li> 
        <li><strong>页面</strong>：按页面，从首页到最后一页，或从最后一页到第一页</li> 
        <li><strong>创建者</strong>：根据添加它们的用户的名称，从A-Z到Z-A</li> 
       </ul> <p>这些选项不会影响导出为XLS或PDF文件的输出。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">评论过滤条件</td> 
      <td> <p>您可以使用这些选项的任意组合，在打印或导出为XLS或PDF文件的输出中仅包含某些注释：</p> 
       <ul> 
        <li>您选择的作者（默认）</li> 
        <li>您选择的操作</li> 
        <li><strong>未解析</strong>状态</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作流</td> 
      <td> <p>（仅当验证具有自动工作流时可用）您可以单击<strong>显示图表</strong>以在打印输出中包含一个图表，该图表显示验证阶段以及在每个阶段做出的决策。 在显示的图表中，颜色表示在舞台上做出的决策：</p> <p><strong>绿色</strong>：已批准</p> <p><strong>蓝色</strong>：正在等待决定</p> <p><strong>红色</strong>：需要做出更改决定</p> <p><strong>灰色</strong>：尚未开始</p> <p><strong>黄色</strong>：已批准，但有更改</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**打印**。
1. 在出现的窗口的右侧面板中，如果要打印摘要，请单击&#x200B;**目标**&#x200B;菜单，然后单击&#x200B;**查看更多**。 在显示的列表中单击要使用的打印机，然后单击&#x200B;**打印**。

   或

   如果要将摘要另存为PDF文件，请单击&#x200B;**目标**&#x200B;菜单，单击&#x200B;**另存为PDF**，然后单击&#x200B;**保存**。

## 将验证摘要导出为XLS或PDF

您可以将静态内容的验证摘要导出为XLS文件或PDF文件。 验证导出仅包括验证的内容。

1. 在包含验证的文档列表中，将鼠标悬停在包含该文档的行上，然后单击&#x200B;**打印摘要**。

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. 单击页面右上角附近的XLS图标或PDF图标。

   ![XLS PDF图标](assets/xls-pdf-icons-350x136.png)

当导出的文件准备就绪时，您将收到一封电子邮件，您可以从其中下载文件。

如果将摘要导出为PDF文件，则PDF阅读器中会显示有关校样的备注。 如果评论具有多个关联的标记，则该评论将在评论列表中多次出现（每个标记出现一次）。
