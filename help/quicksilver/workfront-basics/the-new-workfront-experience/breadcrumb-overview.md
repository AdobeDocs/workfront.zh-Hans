---
content-type: overview
title: 痕迹导航概述
description: 痕迹导航显示所有对象类型的完整导航层次结构。
feature: Get Started with Workfront
exl-id: c4103f8e-4c3f-4d4d-a0eb-628c60735ab7
source-git-commit: 0fea13b0a1d8f14c2d601e0ed0a8d15684a3c4d7
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 0%

---

# 痕迹导航概述

痕迹导航显示所有对象类型的完整导航层次结构。 痕迹导航路径中的每个对象都有一个显示对象类型的标签。 当前所在的页面以斜体显示在页眉和痕迹导航路径末尾。 在以下示例中，这是“[!UICONTROL 与品牌团队]共享”任务。

![折叠的痕迹导航](assets/NWE-collapsed-breadcrumb.png)

当痕迹导航路径中的对象过多或屏幕宽度禁止显示完整导航层次结构时，路径会折叠某些痕迹导航，并在痕迹导航路径的开头对这些对象进行分组。 项目页面和当前对象页面在痕迹导航路径中始终可见。

例如，上图中的“其他3个”表示3个对象未显示。 这些项目可以位于项目级别的上方或项目与当前页面之间。

单击“[!UICONTROL 更多]”可展开整个层次结构。 您可以单击“[!UICONTROL 更少]”以再次折叠痕迹导航路径。

![扩展的痕迹导航](assets/NWE-expanded-breadcrumb.png)

您还可以使用以下键在痕迹导航中导航：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>选项卡</strong> </td> 
   <td> <p>导航到痕迹导航中的每个项目</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>进入</strong> </td> 
   <td> <p>展开折叠的痕迹导航路径，折叠展开的痕迹导航路径，并在出现对象链接时打开新页面</p> </td> 
  </tr> 
 </tbody> 
</table>

+++访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL Request]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有什么计划或许可证类型，请与[!DNL Workfront]管理员联系。

+++

<!--drafted: this is no longer possible, since we removed Campaigns, but it might come back as part of Maestro: 

## Multi-object breadcrumbs

>[!NOTE]
>
>The information in this article is available only in the Preview environment when you participate in the [!UICONTROL Campaigns] beta program. The functionality described here might not be fully available yet. For more information about current available features and how to enroll, see [Campaigns beta].

Some objects can belong to multiple parent objects. For example, a project can belong to multiple campaigns. In this case, all the campaigns that the project belongs to display in the breadcrumb.

The multi-object listing in the breadcrumb (for example, the campaigns) displays the number of parent objects which expands into a list to display all the campaigns that the project is associated with. For more information, see [Add objects to a campaign](../../manage-work/campaigns/add-objects-to-a-campaign.md).


![Project with multiple campaigns in the breadcrumb](assets/project-with-multiple-campaigns-in-breadcrumb.png)

-->

## 从痕迹导航访问父对象

有关[!DNL Workfront]中父对象的信息，请参阅[了解 [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)中的对象。

1. （视情况而定）如果在折叠的痕迹导航路径中看不到要导航到的对象，请单击&#x200B;**[!UICONTROL 更多]**，然后找到该对象。

   >[!NOTE]
   >
   >如果您没有对象的权限，则该对象在痕迹导航中不可见。

1. 单击痕迹导航路径中的任意对象以访问该对象。

   此时将打开对象页面。
