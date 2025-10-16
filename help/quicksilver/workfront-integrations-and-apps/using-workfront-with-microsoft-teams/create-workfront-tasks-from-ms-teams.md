---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: 创建来自 [!DNL Adobe Workfront] 团队的 [!DNL Microsoft] 任务
description: 如果团队所有者已为您的团队安装和配置 [!DNL Workfront] 的Adobe，并且您从Microsoft Teams登录Workfront，则您可以在Microsoft Teams [!DNL Workfront] 中从Microsoft Teams创建个人任务。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 31b86c8d-967a-446a-86f2-3d38e44c45e1
source-git-commit: 4cf780aa1b1221cd6ff8e6ce58fbb7d3621f7fa9
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 从[!DNL Adobe Workfront]创建[!DNL Microsoft Teams]任务

>[!IMPORTANT]
>
>由于[Microsoft将过渡到“新团队”客户端](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability)，因此Classic Teams客户端在2025年7月1日后将不再可用。 要继续使用Microsoft Teams和Workfront等集成应用程序，客户必须在此日期之前过渡到新团队客户端。
>
>更新的Workfront集成现已可用，并与新团队体验完全兼容。 在大多数情况下，用户完成过渡后，Workfront会自动显示。 如果不包含，则可以从Microsoft Teams App Store手动安装集成。 若要在New Teams客户端中安装或验证Workfront集成，请参阅[安装 [!DNL Adobe Workfront] Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。



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
   <td> <p>标准</p>
   <p>工作或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

如果满足以下条件，则可以从[!DNL Adobe Workfront]在[!DNL Microsoft Teams]中创建个人任务：

* 团队所有者已为您的团队安装和配置[!DNL Workfront for Microsoft Teams]。
* 您已从[!DNL Workfront]登录[!DNL Microsoft Teams]。

>[!NOTE]
>
>[!DNL Microsoft Teams]不再支持[!DNL Internet Explorer]。 要使用[!DNL Adobe Workfront for Microsoft Teams]集成，您必须使用[!DNL Internet Explorer]以外的Web浏览器。

有关安装[!DNL Workfront for Microsoft Teams]以及从[!UICONTROL 登录到]Workfront[!DNL Microsoft Teams]的信息，请参阅[安装 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

## 从[!DNL Microsoft Teams]创建个人任务

1. 从[!DNL Workfront]登录到[!DNL Microsoft Teams]。

   有关登录到[!DNL Workfront]的信息，请参阅[安装 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

1. 要打开&#x200B;**[!UICONTROL 新任务]**&#x200B;信息卡：

   * 如果您在[!DNL Workfront]机器人聊天频道，请在&#x200B;**[!UICONTROL 对话]**&#x200B;字段中键入[!UICONTROL 新任务]以创建新任务。
   * 如果您在[!DNL Workfront]机器人聊天频道以外的聊天频道：

      * 开始在&#x200B;**[!DNL @workfront]**&#x200B;对话[!UICONTROL 字段中键入]，然后选择所需的[!DNL Workfront]机器人渠道。
      * 继续在&#x200B;**[!UICONTROL 对话]**&#x200B;字段中键入[!UICONTROL 新任务]以创建新任务。

        [!UICONTROL 新任务]信息卡显示在[!DNL Workfront]机器人渠道中。

        ![ms_teams_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. 在[!UICONTROL Workfront]机器人渠道中，在[!UICONTROL 新建任务]信息卡上指定以下信息：

   * **[!UICONTROL 中的任务名称编写任务的标题]**&#x200B;字段。
   * 在&#x200B;**[!UICONTROL 编写任务的描述]**&#x200B;字段中的任务描述。
   * 任务必须在&#x200B;**[!UICONTROL 到期日期]**&#x200B;字段中完成的日期。

1. 单击&#x200B;**[!UICONTROL 保存]。**

   新的个人任务在[!DNL Workfront]中创建。 [!UICONTROL 参考编号]已分配给它并在[!UICONTROL 新任务]信息卡上可见。

   有关参考编号的信息，请参阅[[!UICONTROL 了解]文章中的对象中的](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects)参考编号[对象部分 [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)。

1. （可选）单击&#x200B;**[!UICONTROL 编辑]**&#x200B;以进一步编辑任务信息。
1. （可选）单击&#x200B;**[!UICONTROL 在[!DNL Workfront]]**&#x200B;中查看以在[!DNL Workfront]的新选项卡中打开该任务，然后进一步编辑该任务，将其移动到项目中，或将其分配给其他人。
