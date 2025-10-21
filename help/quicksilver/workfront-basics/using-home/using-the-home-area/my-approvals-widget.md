---
product-area: home
navigation-topic: use-the-home-area
title: 使用我的审批构件管理您的审批
description: “我的审批”小组件在一个位置显示所有待处理、已分配、已委托和已提交的审批。 在这里，您可以根据需要筛选和组织审批、做出决策并委派审批。
author: Courtney
feature: Get Started with Workfront
source-git-commit: 4981d9adb2cae53e30f13aa2a7aa6857befbf3ca
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 5%

---

# 使用我的审批构件管理您的审批

“我的审批”小组件在一个位置显示所有待处理、已分配、已委托和已提交的审批。 在这里，您可以根据需要筛选和组织审批、做出决策并委派审批。

我的审批小组件支持来自以下Workfront对象的审批：

* 任务
* 问题
* 项目
* 文档
* 校样
* 计划记录请求
* 时间表

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
   <p>参与者或更高版本</p>
   <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看或更高权限访问与审批关联的对象</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看与审批关联的对象的权限或更高的权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 批准我的审批小部件中的工作

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）单击&#x200B;**自定义**&#x200B;以添加&#x200B;**我的审批**&#x200B;小组件。
1. （视情况而定）单击&#x200B;**筛选器**&#x200B;下拉菜单，然后选择&#x200B;**全部**&#x200B;以查看分配给您的审批和委托给您的审批。

   >[!NOTE]
   >
   >分配给工作角色或组的审批不显示在主页中。 分配给团队的审批将显示在每个团队成员的“我的审批”小部件中。


1. 选择要在其中作出批准决策的项目。

   ![我的审批小组件](assets/my-approvals-widget.png)

1. 在右侧面板中作出批准决策时，单击其中一个可用选项。 根据要批准的项目类型，以下选项将显示在页面的右上角：

   <table>
   <tr>
      <td>
      <p><strong>访问</strong></p>
      </td>
      <td>
      <p><strong>工作项</strong></p>
      </td>
      <td>
      <p><strong>文档</strong></p>
      </td>
      <td>
      <p><strong>校样</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>授权</li>
      <li>忽略</li>
      </ul>
      如果需要，您可以在<b>更改访问权限</b>下拉菜单中调整访问级别。
      </td>
      <td>
         <ul>
         <li>批准</li>
         <li>Reject</li>
         </ul>
      您可以通过单击决策按钮中的下拉菜单来在决策中保留评论。
      </td>
      <td>
   已指定为审批者
         <ul>
         <li>批准</li>
         <li>批准（附加更改）</li>
         <li>需要工作</li>
         </ul>
   已分配为审阅者
         <ul>
         <li>完成我的审阅</li>
         </ul>
      此列中的选项仅适用于“统一审批”。 旧文档审批与工作项审批显示相同。 
      </td>
      <td>
         <ul>
         <li>前往校对</li>
         </ul>
         您在验证查看器中做出决定。 有关审阅校样的信息，请参阅<a href="/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">在Adobe Workfront中审阅校样</a>。
      </td>
   </tr>
   </table>

作出决定后，批准将从“我的批准”构件中删除。