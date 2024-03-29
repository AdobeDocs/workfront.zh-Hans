---
product-area: betas
navigation-topic: new-commenting-experience-beta
title: 新的评论体验
description: Adobe Workfront中的评论体验更新目前正在开发中。 此更新包括新界面、新功能和所选对象更新部分中的改进性能。
author: Alina
feature: Product Announcements
role: User
exl-id: f750b35b-8021-4cc1-81d6-e1ece2530438
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '1317'
ht-degree: 2%

---

# 新的评论体验

<!--take out legacy, preview, prod references from below-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.  </span>  

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](../../product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>-->

<!--

After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases.

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  -->

>[!IMPORTANT]
>
>本文中的信息是指已发布到新评论体验的功能。
>
>新评论体验测试版计划于2023年4月开始，于2023年10月结束。 新评论体验的Beta测试版计划已于2023年10月版结束。
>
>从2023年10月开始，所有新评论体验的新功能均已发布给所有客户。 有关更多信息，请参阅每个版本的当前版本概述页面。

<!--An update to the commenting experience in Adobe Workfront is currently in development. This update includes a new interface, new features, and improved performance in the Updates section of select objects. 

The new commenting experience will slowly become available for all the objects with an Updates section in Workfront, and later it will expand to other Adobe Experience Cloud applications.-->

<!--For additional resources for the new commenting experience, also see the following articles:

* [New commenting experience release activity](../new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md)
* [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md)
-->

## 功能

新的评论体验包括对Adobe Workfront对象更新部分的改进和更改。

新评论体验中包括的改进包括：

* 改进了性能和用户体验
* 将用户评论与系统活动更新分离
* 向对象添加新注释时的实时指示器
* 提交评论后进行编辑

以下功能已从新Experience中删除或将被弃用：

* 有关系统更新的注释
* 在评论任务和问题时能够编辑状态、条件、提交日期和完成百分比
* 编辑自定义表单
* 当Workfront或组管理员以其他用户身份登录并为其添加评论时，“代表&lt;用户名>”信息最初被删除。 它已于2023年10月19日恢复。
* 在向文档添加评论时标记人员时的“请求审批”选项。
* 编辑用户配置文件框时的“显示更新状态的完成百分比”设置将被删除。 已删除更新任务或问题的完成百分比的功能。
* 更新区域中的项目所有者通知，任务或问题的任务接受者编辑了提交日期 <!--ensure this is correct when re remove the legacy and leave only new commenting-->

<!--removed this note on November 28, 2023, when this limitation was removed: 

>[!NOTE]
>
>The objects listed below have only the comments and system updates starting with January 1, 2019 available in the new commenting experience.  
>
>You can view comments and system updates on these objects prior to January 1, 2019 when viewing the Updates section in the current experience:
>
>* Issues
>* Projects
>* Tasks
>* Documents

For more information, see the [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md). 
-->

下表说明了新Commending Experience中可用的功能以及这些功能在受支持领域的可用性：

<table>
  <tr>
   <td><strong>功能 </strong>
   </td>
   <td><strong>存在于旧评论体验中 </strong>
   </td>
   <td><strong>存在于新的评论体验中 </strong>
   </td>
   <td><strong>将在新的评论体验中引入 </strong>
   </td>
   <td><strong>何时将在新的评论体验中引入 </strong>
   </td>
   <td><strong>正在研究 </strong>
   </td>
  </tr>
  <tr>
   <td>创建/读取/回复/删除评论 
   </td>
   <td>✓ {\f13 } 
  </td>
   <td>✓ {\f13 } 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>富文本（不包括引号和表情符号）
   </td>
   <td>✓ {\f13 } 
   </td>
   <td>✓ {\f13 }
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>富文本（表情符号）
   </td>
   <td>✓ {\f13 } 
   </td>
   <td>✓ {\f13 }
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>富文本（块引号）
   </td>
   <td>✓ {\f13 } 
   </td>
   <td> ✓ {\f13 }
   </td>
   <td> 
   </td>
   <td> 2023年第二季度
   </td>
   <td> 
   </td>
  </tr>
  <tr>
<tr>
   <td> 报价注释
   </td>
   <td>✓ {\f13 } 
   </td>
   <td> ✓ {\f13 }
   </td>
   <td> 
   </td>
   <td> 2023年第二季度
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>对评论做出反应（类似） 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>将图像附加到注释 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>在评论中标记人员 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>删除线程参与者
   </td>
   <td> 
   </td>
   <td>✓ {\f13 }
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>


<tr>
   <td>自动标记所有线程参与者
   </td>
   <td> 
   </td>
   <td>✓ {\f13 }
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>公司私有的评论 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>撤消评论的过帐 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td>替换为编辑注释 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>关闭系统更新 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td>已替换为活动选项卡 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>编辑评论 
   </td>
   <td> 
   </td>
   <td> ✓ {\f13 }
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>在离开页面时保存评论草稿 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>实时查看新评论（包括查看何时删除评论）
   </td>
   <td> 
   </td>
   <td>✓ {\f13 }
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>记录时间 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td>✓ {\f13 }
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>复制跟帖链接 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td> 替换为复制链接
   </td>
   <td> 
   </td>
   <td>2023年第二季度 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>复制评论链接 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td> 替换为复制链接
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>引用注释文本 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td>✓ {\f13 }
   </td>
   <td> 
   </td>
   <td>2023年第二季度 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>复制正文文本 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td> ✓ {\f13 }
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>在评论中搜索 
   </td>
   <td> 
   </td>
   <td> ✓ {\f13 }
   </td>
   <td> 
   </td>
   <td>2024年第一季度 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>在评论中复制并粘贴图像
   </td>
   <td> 
   </td>
   <td> ✓ {\f13 }
   </td>
   <td> 
   </td>
   <td>2024年第一季度 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>在评论中拖放图像
   </td>
   <td> ✓ {\f13 }
   </td>
   <td> ✓ {\f13 }
   </td>
   <td> 
   </td>
   <td>2024年第一季度 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>编辑自定义表单 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>在注释时编辑状态、条件和提交日期的功能 
   </td>
   <td>✓ {\f13 } 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>
   </td>
  </tr>
<tr>
   <td>回复系统更新 
   </td>
   <td> ✓ {\f13 }
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
<tr>
   <td>添加以其他用户身份登录的评论时显示“代表”
   </td>
   <td> ✓ {\f13 }
   </td>
   <td> ✓ {\f13 }
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
</table>

## 发布时间表

>[!IMPORTANT]
>
>有关在Beta测试版时间范围内向新评论体验发布的功能的信息，请参阅 [新的评论Beta版体验发布活动](../../betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md).
>
>有关管理Workfront对象更新的更多信息，请参阅 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


以下是向生产环境发布新评论体验的计划时间线，其中具有关键里程碑。 除了下面的里程碑之外，我们将继续通过较小的增强功能改进评论体验。

有关在Beta版结束之后为新评论体验发布的功能的信息，请参阅当前版本概述页面。

以下是发布新评论体验的计划时间表：

* 在23.2版本（2023年4月6日）中：
   * 针对问题启动评论体验Beta版
   * 发布新的目标评论体验（作为唯一体验）
* 在23.3版本（2023年7月20日）中：
   * 为项目、任务和文档启动评论体验测试版。
   * 在展示板区域发布信息卡的新评论体验（作为唯一体验）
* 在2023年第四季度版本（限量版本，仅向选择快速版本的客户提供）中：
   * 发布模板、模板任务、程序、项目组合、团队、用户和工时表的新评论体验（作为唯一体验）
   * 更新项目、任务、问题和文档的评论体验测试版，使其成为默认选项。 移除“Beta”标签。
* 在2023年第四季度(23.10)发布（2023年10月26日）
   * 向所有客户发布有关模板、模板任务、程序、项目组合、团队、用户和工时表的新注释体验（作为唯一体验）。
   * 将项目、任务、问题和文档的新注释体验设置为默认选项。

  >[!IMPORTANT]
  >
  >    这将结束新评论体验的Beta阶段。

   * 从这一日期开始，将针对新评论体验发布的所有功能纳入当前的每月和季度定期发布中。
* 2023年底：
   * 将旧版注释体验保留为以下对象的辅助选项：项目、任务、问题和文档。 新注释体验是这些对象的所有用户的默认选项。
   * 使新的注释体验成为所有其他对象的唯一体验。

  >[!NOTE]
  >
  >    迭代将继续具有旧版评论体验。 新的评论体验将不可用于迭代。

* 2024年第二季度（2024年4月）：

   * 删除切换回旧版注释流的选项，并使新注释流成为所有对象的唯一体验，迭代除外。

## 找到新的评论体验

&lt;! — 重要提示：当我们删除旧版体验时，请将此体验的一个版本移至“更新”工作文章或“更新”部分概述 — 也就是说，除了迭代之外，其他所有体验都不同 — >

新的评论体验目前向所有客户和所有环境提供。

根据您访问评论体验的对象，您可能会看到更新部分的以下功能：

* 以下对象的新注释体验和旧注释体验：

   * 项目
   * 任务（包括故事）
   * 问题
   * 文档

  >[!TIP]
  >
  >使用新注释选项可显示新的注释体验（在启用时）或旧版注释体验（在禁用时），如本节所述。 默认使用新的评论体验。

   * 只有下面列出的对象的新注释体验。 没有选项可为这些对象启用旧版注释体验：

      * 目标

     >[!NOTE]
     >
     >您必须具有Adobe Workfront目标的其他许可证才能访问Workfront的此区域。 有关更多信息，请参阅 [使用Workfront Goals的要求](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
      * 展示板上的信息卡
      * 团队
      * 模板
      * 模板任务
      * 时间表
      * 项目群
      * 项目组合
      * 用户

* 仅限以下对象的旧版注释体验：

   * 迭代

     没有选项可为迭代启用新的评论体验。 只有旧版评论体验可用于迭代。


<!--before August 17: 

The new commenting experience is currently supported for the following objects:


* When enabling the Beta experience in the Updates section for 

    * Issues, projects, tasks, and documents

    For more information about managing updates for Workfront objects, see [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

* By default, as the only commenting experience for

    * Goals, cards on a board

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

-->

<!--Depending on the environment you access the commenting experience you can do one of the following: 

* Enable the commenting experience Beta in the Production environment
* <span class="preview">Enable the legacy commenting experience in the Preview  environment </span>
-->

要为项目、任务、问题和文档启用注释体验选项，请执行以下操作：

1. 转到要为其激活新评论体验的对象，然后单击 **更新** 在左侧面板中。
1. （视情况而定）如果已禁用，请启用 **新建注释** 选项启用该功能。 默认情况下，应该启用此功能。

   ![](assets/new-commenting-toggle-off-highlighted.png)

1. 在中开始键入更新 **评论** 选项卡。 “评论”选项卡是打开新体验时的默认选项卡

   或

   单击  **系统活动** 选项卡中，用于查看Workfront生成的活动更新。

1. （可选）要禁用新的注释体验并返回旧版注释，请取消选择 **新建注释** 选项。

