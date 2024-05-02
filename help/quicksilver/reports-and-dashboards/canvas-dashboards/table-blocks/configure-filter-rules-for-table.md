---
title: 在报告画布中过滤表
description: 在报告画布中过滤表
hidefromtoc: true
hide: true
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 0%

---

# 在报告画布中过滤表

向报表中添加表块后，可以设置过滤器以限制表中显示的信息。

过滤器规则包含3个组件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">字段</td> 
   <td> <p>包含要用于筛选表格信息的字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作员</td> 
   <td> <p>过滤器确定表中包含或排除的字段值的方法。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">值</td> 
   <td> <p>根据运算符计算的选定字段中的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

**示例：** 如果您希望将报告中的结果限制为仅显示Jane Doe拥有的项目，则可以创建一个筛选规则，其中字段“项目所有者”、运算符“等于”和值“Jane Doe”。

或者，您只能显示具有已分配项目所有者的项目，这些已分配项目所有者将具有“项目所有者”字段和运算符“不为空”。

## 先决条件

在开始之前，您必须注册报告画布测试版。 有关更多信息，请参阅 [报告画布测试版：概述](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 配置表的过滤规则

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击&#x200B;**报表**.

1. 单击 **新报告**.

   或

   转到现有报表，单击 **更多菜单** 图标 ![](assets/more-icon.png) 在报表标题中，然后选择 **编辑**.

1. 要将新表中的行分组，请将表块拖动或双击到画布上。

   或

   要对现有表中的行进行分组，请单击 **编辑** 图标 ![](assets/edit-icon.png) 在表标题中。

1. 在右侧面板中，找到要用于筛选表的字段，然后将其拖到筛选条件部分。

   此时将显示一个筛选器规则集，其中包含您选择的字段的名称。

1. 从下拉菜单中选择所需的运算符：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>等于</strong> </td> 
      <td> <p>这仅返回与搜索值完全匹配的值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>不等于</strong> </td> 
      <td> <p>这仅返回与搜索的值不完全匹配的结果。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>为空</strong> </td> 
      <td> <p>对象存在字段，但尚未为该字段赋值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>不为空</strong> </td> 
      <td> <p>您正在筛选的字段已存在并已获得一个值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>小于</strong> </td> 
      <td> <p>这将搜索其值小于输入值的所有结果，而不包括输入的值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>小于或等于</strong> </td> 
      <td> <p>这将搜索其值小于或等于输入值的所有结果。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>大于</strong> </td> 
      <td> <p>这将搜索其值大于输入值的所有结果，而不包括输入值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>大于或等于</strong> </td> 
      <td> <p>这将搜索其值大于或等于输入值的所有结果。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>介于</strong> </td> 
      <td> <p>提供2个必填字段值，并在两个字段（包括输入的值）范围内搜索所有结果。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>包含</strong> </td> 
      <td> <p>在整个文本字符串中搜索指定的文本。</p> <p>例如，使用“包含Inf”会捕获其中包含“Inf”或“inf”的任何内容，例如“Infinity”一词。</p> <p>注意：Adobe Workfront将搜索您为每个过滤规则输入的整个单词或短语。 例如，如果您要搜索名称中包含“new project”短语的字段，Workfront不会显示名称中仅包含“new”或“project”的项目，也不会显示包含中间额外单词的短语，如“new main project”。 该过滤器仅查找名称中具有精确短语“新项目”的项目。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>不包含</strong> </td> 
      <td> <p>这会过滤掉缺少指定文本的项目。</p> <p>例如，“不包含inf”会返回名称中不带“Inf”或“inf”的任何字段。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 根据所选的运算符，输入完成筛选规则的最后一个值。

   >[!NOTE]
   >
   >此处输入的值为 **非** 区分大小写。

1. （可选）要将其他筛选规则添加到规则集，请执行以下操作：

   1. 将另一个字段拖到 **放置以添加另一个规则** 区中其他规则下方的过滤器区域。
   1. 重复步骤4 - 6。
   1. 在新规则的左侧运算符下拉菜单中，选择 **和** 或 **或者**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>和</p> </td> 
         <td> <p>使用AND运算符连接过滤器规则或规则集时，会指示希望满足同一级别的所有规则。</p> <p>默认情况下，过滤器中的语句使用AND运算符连接。</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>或</p> </td> 
         <td> <p>使用OR运算符连接过滤器规则或规则集时，会指示您需要 <strong>至少</strong> 一个规则（或规则集）。</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >同一级别的AND和OR运算符（将规则集中的多个规则或整个规则集连接在一起）始终匹配。 例如，如果更改规则集中两个规则之间的运算符，则该规则集中的所有其他运算符都将自动更改以匹配该运算符。

1. （视情况而定）要添加额外的筛选规则集，请执行以下操作：

   1. 将要添加的字段拖到 **添加规则集** 其他筛选规则集下方的区域。
   1. 重复步骤4 - 7。
   1. 在新规则集左侧的运算符下拉菜单中，选择 **和** 或 **或者**. 这些运算符的功能与步骤7中列出的运算符相同，但适用于整个规则集，而不是规则集中的单个规则。****
