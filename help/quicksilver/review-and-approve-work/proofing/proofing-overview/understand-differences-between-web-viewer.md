---
content-type: reference
product-area: documents
navigation-topic: proofing-overview
title: Web验证查看器和桌面验证查看器的区别概述
description: 了解桌面和网页验证查看者之间的差异。
author: Courtney
feature: Digital Content and Documents
exl-id: 72ce147b-29c9-4c3b-a03c-2da0758bc178
TQID: https://experienceleague.adobe.com/5wUR3OHvmgjQmRtvt85iax2gbY0rC0yWsLzuLULia3M
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c2be0313-b3ae-45e0-b454-d20bf54b23f2id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 872
ht-degree: 5%

---

# Web验证查看器和桌面验证查看器的区别概述

Adobe Workfront提供两种不同的验证查看器：

* **Web校对查看器：**&#x200B;主要用于校对静态文件和视频文件。 在Google Chrome、Firefox或Safari中运行。
* **桌面校对查看器：**&#x200B;专为校对交互式文件以及视频和静态文件而设计。 作为独立应用程序在工作站上运行。 有关详细信息，请参阅[了解桌面校对查看器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md)

* 如果您的组织出于安全原因无法使用桌面验证查看器应用程序，则Workfront管理员可以配置您的系统，以便您可以在Web验证查看器中查看捆绑在ZIP存档文件中的交互式内容。 有关详细信息，请参阅[在Web验证查看器中设置交互式内容验证](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md)。

以下列表可帮助您了解可用于验证特定内容类型的验证查看者：

* **交互式Web内容 — URL**：如果您使用URL为Web内容创建校对，并且希望以交互方式校对内容，则必须使用桌面校对查看器。
* **交互式Web内容 — ZIP文件**：如果您使用ZIP文件为Web内容创建校对，则可以使用Web校对查看器（存在一些限制）或桌面校对查看器。 有关将Web验证查看器用于交互式内容所涉及的限制的信息，请参阅[在Web验证查看器中设置交互式内容验证](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md)。

* **静态内容和视频内容**：如果您创建的校对包含静态内容，则可以使用Web校对查看器或桌面校对查看器。

## 静态校样

| **功能** | **Web验证查看器** | **桌面校对查看器** |
|---|---|---|
| 打开静态校样 | ✓ | ✓&#42; |
| 单视图、杂志视图和连续视图 | ✓ | ✓&#42; |
| 平移 | ✓ | ✓&#42; |
| 缩放 | ✓ | ✓&#42; |
| 旋转 | ✓ | ✓&#42; |
| 测量工具 | ✓ （设置自定义大小的区域） | ✓&#42; |
| 缩略图视图 | ✓ | ✓&#42; |
| 静态校对导航器 | ✓ | ✓&#42; |
| 文档搜索 | ✓ | ✓&#42; |
| 在多个页面上发布评论 | ✓ （在所有视图中可用） | ✓&#42; （在所有视图中可用） |
| 高级静态校对快捷键 | ✓ （有关详细信息，请参阅验证查看器中的[键盘快捷键](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)） | ✓&#42;（有关详细信息，请参阅验证查看器中的[键盘快捷键](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)） |

{style="table-layout:auto"}

&#42;仅当Workfront管理员将桌面校对查看器配置为所有校对的默认查看器时，此功能才有效。

## 视频校样

| **功能**  | **Web验证查看器** | **桌面校对查看器** |
|---|---|---|
| 打开视频校样 | ✓ | ✓&#42; |
| 缓冲 | ✓ | ✓&#42; |
| 使用时间复查 | ✓ | ✓&#42; |
| 使用时间范围或时间代码进行审阅 | ✓ | ✓&#42; |
| 快速或慢速查看 | ✓ | ✓&#42; |
| 音量调节 | ✓ | ✓&#42;  |
| 全屏模式 | ✓ | ✓&#42;  |
| 范围注释 | ✓ | ✓&#42;  |
| 循环视频校样（视频完成和自动开始） | ✓ | ✓&#42;  |
| 高级视频快捷键 | ✓ （有关详细信息，请参阅验证查看器中的[键盘快捷键](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)） | ✓&#42;  |

{style="table-layout:auto"}

&#42;仅当将桌面校对查看器配置为所有校对的默认查看器时，此功能才有效。

## 交互式校样

| **功能**  | **Web验证查看器** | **桌面校对查看器** |
|---|---|---|
| 打开通过ZIP文件中捆绑的内容创建的交互式验证 | ✓ | ✓ （推荐） |
| 打开从URL创建的交互式验证 | 不受支持 | ✓ |
| 查看各种屏幕大小的交互式校样（从ZIP文件中捆绑的内容创建） | ✓ | ✓ |
| 查看各种设备的交互式验证（从ZIP文件中捆绑的内容创建） | 不受支持 | ✓ |
| 审查不安全(HTTP)站点 | 不受支持 | ✓ |
| 查看受iFrame保护的网站（受保护、无法在iFrame中查看的网站） | 不受支持 | ✓ |

{style="table-layout:auto"}

## 评论

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>功能</th> 
   <th>Web验证查看器 </th> 
   <th>桌面校对查看器 </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>添加、删除和编辑评论</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>添加和删除回复</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>矩形、箭头、线条、手绘和突出显示标记工具</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>折线工具</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>裁切蒙版标记工具</p> </td> 
   <td>不受支持</td> 
   <td>不受支持</td> 
  </tr> 
  <tr> 
   <td> <p>文本选择标记工具</p> </td> 
   <td>仅✓用静态验证</td> 
   <td>仅✓用静态验证</td> 
  </tr> 
  <tr> 
   <td> <p>更改标记颜色</p> </td> 
   <td>✓（有32种颜色可用） </td> 
   <td>✓（有32种颜色可用） </td> 
  </tr> 
  <tr> 
   <td> <p>更改标记不透明度</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>更改标记粗细</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>剪切、复制和粘贴标记</p> </td> 
   <td> 不受支持</td> 
   <td> 不受支持</td> 
  </tr> 
  <tr> 
   <td> <p>撤消和重做上一个操作</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>复制标记</p> </td> 
   <td> 不受支持</td> 
   <td> 不受支持</td> 
  </tr> 
  <tr> 
   <td>将操作设置为注释</td> 
   <td>✓（设置操作后，立即可在评论上看到操作）</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>将标记颜色设置为默认值</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>解决评论</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>锁定评论</p> </td> 
   <td>不受支持</td> 
   <td> 不受支持</td> 
  </tr> 
  <tr> 
   <td> <p>标记用户</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>恢复评论</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>在紧凑视图中查看评论列表</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>在标准、完整或单个视图中查看注释列表</p> </td> 
   <td>为将来计划</td> 
   <td>为将来计划</td> 
  </tr> 
  <tr> 
   <td> <p>搜索评论</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>按用户过滤注释</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>按用户过滤评论和回复</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>为评论排序</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>评论自动更新</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## 决策

| 功能 | Web验证查看器 | 桌面校对查看器 |
|---|---|---|
| 制定决策 | ✓ | ✓ |
| 自定义决策 | ✓ | ✓ |

{style="table-layout:auto"}

## 比较校样

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>功能</th> 
   <th>Web验证查看器 </th> 
   <th>桌面校对查看器 </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>比较不同版本的验证</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
  <tr> 
   <td>比较单独的校样</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

## 校对操作

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>功能</th> 
   <th>Web验证查看器 </th> 
   <th>桌面校对查看器 </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>更改校对版本 </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td>创建新版本</td> 
   <td> <p>仅在Workfront Proof中可用（将来计划在Workfront中校对时）<br></p> </td> 
   <td>仅在Workfront Proof中可用（将来计划在Workfront中校对时）</td> 
  </tr> 
  <tr> 
   <td>查看校对详细信息 </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>审核验证工作流</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>编辑工作流暂存</td> 
   <td>不受支持</td> 
   <td>不受支持</td> 
  </tr> 
  <tr> 
   <td>共享校样</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>获取团队URL</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>更改电子邮件通知</td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>下载原始文件</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>锁定和解锁验证和暂存</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>打印校对摘要</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>删除校样</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>从同一文件夹管理校样</td> 
   <td><strong>仅在Workfront Proof中可用</strong> </td> 
   <td><strong>仅在Workfront Proof中可用</strong> </td> 
  </tr> 
  <tr> 
   <td>品牌策略（自定义徽标）</td> 
   <td>✓</td> 
   <td> ✓<br>（启动页面上的Workfront徽标） </td> 
  </tr> 
  <tr> 
   <td>自定义链接（仅限Workfront Proof）</td> 
   <td>不受支持</td> 
   <td> 不受支持 </td> 
  </tr> 
  <tr> 
   <td>Basecamp集成（仅限Workfront Proof） </td> 
   <td>为将来计划</td> 
   <td>为将来计划</td> 
  </tr> 
  <tr> 
   <td>状态指示器 </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>验证自动更新（权限更改和新版本）</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
 </tbody> 
</table>

## 微型查看器

| **功能**  | **Web验证查看器**  | **桌面校对查看器** |
|---|---|---|
| 嵌入式代码 | 计划在未来推出静态和本机视频校样 | 不受支持  |

{style="table-layout:auto"}

## 翻译

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>功能</strong> </th> 
   <th><strong>Web验证查看器</strong> </th> 
   <th><strong>桌面校对查看器</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>英语以外的支持语言</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
 </tbody> 
</table>
