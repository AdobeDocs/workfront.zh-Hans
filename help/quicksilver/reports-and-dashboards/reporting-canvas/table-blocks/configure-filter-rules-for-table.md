---
title: 在报表画布中过滤表
description: 在报表画布中过滤表
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 1%

---


# 在报表画布中过滤表

在将表块添加到报表后，可以设置过滤器以限制表中显示的信息。

过滤器规则中有3个组件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">字段</td> 
   <td> <p>字段，其中包含用于筛选表的信息。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">运算符</td> 
   <td> <p>过滤器确定表中包含或排除哪些字段值的方式。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">值</td> 
   <td> <p>根据运算符计算的选定字段中的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

**示例：** 如果您希望将报表中的结果限制为仅显示Jane Doe拥有的项目，则可以创建一个筛选规则，其中字段为“项目所有者”，运算符为“等于”，值为“Jane Doe”。

或者，您只能显示已分配项目所有者的项目，该项目将具有字段“项目所有者”和运算符“不为空”。

## 先决条件

在开始之前，您必须注册报表画布测试版。 有关更多信息，请参阅 [报表画布测试版：概述](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## 为表配置过滤器规则

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击&#x200B;**报表**.

1. 单击 **新报告**.

   或

   转到现有报表，单击 **“更多”菜单** 图标 ![](assets/more-icon.png) 在报表标题中，选择 **编辑**.

1. 要在新表上对行进行分组，请将表块拖动或双击到画布上。

   或

   要对现有表上的行进行分组，请单击 **编辑** 图标 ![](assets/edit-icon.png) 在表标题中。

1. 在右侧面板中，找到要通过其筛选表的字段，然后将其拖动到“筛选器”部分。

   此时将显示一个筛选器规则集，其中包含您选择的字段的名称。

1. 从下拉菜单中选择所需的运算符：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>等于</strong> </td> 
      <td> <p>这仅返回与搜索值的完全匹配项。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>不等于</strong> </td> 
      <td> <p>这仅会返回与搜索值不完全匹配的结果。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>空白</strong> </td> 
      <td> <p>该字段存在于对象中，但尚未为该字段赋值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>不为空白</strong> </td> 
      <td> <p>要筛选的字段存在，且已赋值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>小于</strong> </td> 
      <td> <p>这会搜索值小于输入内容的所有结果，而不包括输入的值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Less Than Or Equal To</strong> </td> 
      <td> <p>这会搜索值小于或等于输入值的所有结果。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>大于</strong> </td> 
      <td> <p>这会搜索值大于输入值的所有结果，而不包括输入值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Greater Than Or Equal To</strong> </td> 
      <td> <p>这会搜索值大于或等于输入值的所有结果。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>介于</strong> </td> 
      <td> <p>提供2个必填字段值，并搜索两个字段范围（包括输入的值）内的所有结果。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>包含</strong> </td> 
      <td> <p>这会在整个文本字符串中搜索指定的文本。</p> <p>例如，使用“包含Inf”可捕获其中包含“Inf”或“inf”的任何内容，如“Infinity”一词。</p> <p>注意：Adobe Workfront会搜索您为每个过滤器规则输入的整个单词或短语。 例如，如果您正在搜索名称中带有“new project”字样的字段，则Workfront不会显示名称中只包含“new”或“project”的项目，或中间包含额外词语的短语（如“new main project”）。 过滤器仅会查找名称中具有确切短语“new project”的项目。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>不包含</strong> </td> 
      <td> <p>这会过滤掉缺少指定文本的项目。</p> <p>例如，“不包含inf”会返回名称中没有“Inf”或“inf”的任何字段。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 根据您选择的运算符，输入最后一个值以完成筛选规则。

   >[!NOTE]
   >
   >此处输入的值包括 **not** 区分大小写。

1. （可选）要向规则集添加其他过滤器规则，请执行以下操作：

   1. 将另一个字段拖到 **拖放以添加其他规则** 的“过滤器”区域。
   1. 重复步骤4-6。
   1. 在新规则的运算符下拉列表中，选择 **和** 或 **或**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>和</p> </td> 
         <td> <p>使用AND运算符连接过滤器规则或规则集时，您会指示您希望满足同一级别的所有规则。</p> <p>默认情况下，过滤器中的语句使用AND运算符联接。</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>或</p> </td> 
         <td> <p>使用OR运算符连接过滤器规则或规则集时，您会指示您需要 <strong>至少</strong> 在要满足的级别上有一个规则（或规则集）。</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >同一级别的AND和OR运算符（将规则集中的多个规则或整个规则集中的任意一个连接在一起）将始终匹配。 例如，如果在规则集中的两个规则之间更改运算符，则该规则集中的所有其他运算符将自动更改以匹配它。

1. （视情况而定）要添加其他过滤器规则集，请执行以下操作：

   1. 将要添加的字段拖到 **添加规则集** 区域。
   1. 重复步骤4-7。
   1. 在新规则集的运算符下拉列表中，选择 **和** 或 **或**. 这些运算符的作用与步骤7中列出的运算符相同，但与规则集中的单个规则相反，它们适用于整个规则集。****
