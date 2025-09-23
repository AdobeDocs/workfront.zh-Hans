---
title: AI助手提示最佳实践
content-type: reference
description: 了解使用AI助手的最佳实践，并查看提示示例列表。
author: Jenny
feature: Get Started with Workfront
source-git-commit: 74bdbaa0dd4df7b11a96105ad4258b06317b2510
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 4%

---

# AI助手提示最佳实践

Workfront的AI助手是一款功能强大的工具，可提供有关帐户数据和特定对象类型的有用信息，从而帮助您更有效地完成工作。

在本文中，您将了解AI助理的当前最佳实践，包括如何编写清除提示、可以询问有关哪些对象类型的信息，以及如何在需要时访问其他资源以验证信息。

有关AI助手的详细信息，请参阅[AI助手概述](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)。

>[!NOTE]
>
>随着AI Assistant功能的发展，您可以向其提出的请求和问题类型将会增加。 我们建议在发布新的AI Assistant功能时重新阅读本文，以详细了解您可以使用的可用提示。


## AI助手可用的对象类型

AI助手可以为以下对象类型提供数据：

* 项目组合
* 项目群
* 项目
* 任务
* 问题
* 自定义表单
* 用户
* Workfront Planning记录

>[!NOTE]
>
>您必须具有对象访问级别的必需权限，然后才能从AI助手请求其数据。

## 最佳实践

### 输入清除提示

要从AI Assistant访问最有用的信息，请务必创建提示，为您提供要查找的响应。 以下列表包含可以帮助您最好地制定相应提示的原则：

* **确实使用明确而具体的语言**：避免模糊而一般的提示将有助于指导AI助手获取您尝试接收的数据。
* **包括时间范围**：为对象指定AI助手特定时间范围将有助于缩小需要处理的数据范围，并在其响应中生成更多目标信息。
* **一次只请求一件事**：如果单个提示中包含多个不相关的请求，则AI助手将无法提供正确的信息。

有关推荐提示的信息，请参阅本文中的以下部分：[提示示例](#prompt-examples)。


### 验证AI助手响应

在AI助手开发的这个阶段，建议验证它提供的信息，然后再询问有关Workfront进程的信息。 要执行此操作，请单击即时响应中“源”部分中提供的文章链接。

![源部分](assets/sources-section.png)

有关Workfront进程提示的详细信息，请参阅本文中的[提示以了解Workfront操作](#prompts-to-learn-about-workfront-actions)。


## 提示示例

下表包含一些提示示例，您可以使用这些提示生成有关您所做工作的信息，并详细了解您希望执行的特定Workfront流程或操作。

### 提示查找有关您工作的信息

<table>
    <tr>
        <td><b>对象类型</b></td>
        <td><b>提示</b></td>
    </tr>
        <tr>
        <td>项目</td>
        <td><em>[PROJECT NAME]的到期日期是多长时间？</em>
        </td>
    </tr>
    <tr>
        <td>项目</td>
        <td><em>[项目名称]的状态是什么？</em>
        </td>
    </tr>
    <tr>
        <td>项目 </td>
        <td><em>谁是[PROJECT NAME]的项目所有者？</em></td>
    </tr>
    <tr>
        <td>任务</td>
        <td><em>本周分配给我的任务有哪些？</em></td>
    </tr>
       <tr>
        <td>问题 </td>
        <td><em>哪些未完成问题已分配给我的团队？</em></td>
           <tr>
        <td>用户</td>
        <td><em>谁是[PROJECT NAME]创意团队的成员？</em></td>
    </tr>
           <tr>
        <td>用户 </td>
        <td><em>有多少任务分配给[USER]？</em></td>
    </tr>
   </table>


### 提示了解Workfront操作

<table>
    <tr>
        <td><b>对象类型</b></td>
        <td><b>提示</b></td>
    </tr>
    <tr>
        <td>项目</td>
        <td><em>如何从模板创建新项目？</em>
        </td>
    </tr>
    <tr>
        <td>项目 </td>
        <td><em>项目与项目群之间有何区别？</em></td>
    </tr>
    <tr>
        <td>任务</td>
        <td><em>如何将任务分配给多个用户？</em></td>
    </tr>
       <tr>
        <td>任务</td>
        <td><em>准备好开始状态是什么意思？</em></td>
    </tr>
       <tr>
        <td>问题 </td>
        <td><em>如何将请求转换为任务？</em></td>
    </tr>
           <tr>
        <td>问题 </td>
        <td><em>Workfront中问题的生命周期是怎样的？</em></td>
    </tr>
        </tr>
           <tr>
        <td>问题 </td>
        <td><em>如何升级请求？</em></td>
    </tr>
           <tr>
        <td>文档</td>
        <td><em>如何上传文档的新版本？</em></td>
    </tr>
           <tr>
        <td>文档 </td>
        <td><em>我是否可以设置文档审批工作流？</em></td>
    </tr>
   </table>


## 当前AI Assistant限制

AI Assistant是一个功能强大的工具，但是对于某些类型的问题和请求，它无法提供数据给这个发展阶段的应用。 下表包含AI助手无法显示其数据的提示示例。

<table>
    <tr>
        <td><b>提示类型</b></td>
        <td><b>示例</b></td>
    </tr>
    <tr>
        <td>有关自定义配置的问题</td>
        <td><em>在我们的Workfront实例中运行的是什么自定义集成逻辑？</em>
        </td>
    </tr>
    <tr>
        <td>有关Workfront外部数据的问题 </td>
        <td><em>能否显示今天的Outlook日历？</em></td>
    </tr>
             <tr>
        <td>有关未集成的Adobe产品的问题 </td>
        <td><em>如何从此处编辑Acrobat中的PDF？</em></td>
         <tr>
        <td>需要人为判断的问题</td>
        <td><em>该项目是否应搁置？</em></td>
    </tr>
    </tr>
       <tr>
        <td>批量更新请求</td>
        <td><em>为[USER]重新分配所有过期任务。</em></td>
    </tr>
       <tr>
        <td>预测分析请求</td>
        <td><em>根据我们的历史数据提出新的项目计划。</em></td>
    </tr>
           <tr>
        <td>对高于您的访问级别的信息请求</td>
        <td><em>列出帐户中的所有记帐费率。</em></td>
    </tr>
           <tr>
        <td>包含模糊信息的请求 </td>
        <td><em>修复我的项目。</em></td>
    </tr>
   </table>