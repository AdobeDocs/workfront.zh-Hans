---
title: 使用Workfront Planning记录自动化创建Workfront对象
description: 您可以在Workfront Planning中配置自动化，以便在激活后在Workfront中创建对象。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
source-git-commit: bac3ed2a169e070b541192ab312d4fc1a1b467d1
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---


# 使用Workfront Planning记录自动化创建Workfront对象

您可以在Workfront Planning中配置自动化，以便在激活后在Workfront中创建对象。

您激活了记录中的自动化。 Workfront中的对象已连接到您激活自动的Planning记录。

例如，您可以创建一个接受Workfront Planning营销活动的自动化功能，并在Workfront中创建一个项目以跟踪该营销活动的进度。 该项目将连接到Workfront规划活动。

有关已连接记录的详细信息，请参阅[已连接记录概述](/help/quicksilver/planning/records/connected-records-overview.md)。


## 在Workfront Planning中配置自动化

您必须先在Workfront Planning中配置自动化，然后才能使用它创建Workfront对象。

1. 单击&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)并选择&#x200B;**自动化**。

   将打开可用自动化列表。

1. 单击屏幕右上角的&#x200B;**新建自动化**。
1. 在&#x200B;**按钮文本**&#x200B;字段中，输入要显示在按钮上的文本。 使用自动化创建Workfront对象时，用户将单击此按钮。
1. （可选）要将图标添加到按钮，请从可用选项中选择一个图标。
1. 在&#x200B;**创建**&#x200B;类型的字段中，选择要自动创建的对象。

   可用的对象包括：

   * 项目
   * 项目组合
   * 项目群
   * 组

1. 在&#x200B;**选择要用于项目名称**&#x200B;字段的字段中，选择一个记录字段。 Workfront中的新项目将使用此字段的内容作为名称。
1. 在&#x200B;**选择要链接已创建项目的字段**&#x200B;中，选择一个记录字段。 在Workfront Planning中查看记录时，Workfront中的新项目将显示在此字段中。
1. 选择对正在创建的对象类型可用的其他选项。
1. 单击&#x200B;**创建**

自动化显示在自动化列表中，并可用于记录。

## 使用Workfront Planning自动化创建Workfront对象

1. 在Workfront Planning中，打开包含要用于创建Workfront对象的记录的记录类型页面。
1. 选择一个或多个记录。
1. 单击屏幕右下角附近的自动化按钮。

   在本例中，选择“创建项目”按钮。

   ![自动化按钮](assets/automation-custom-button.png)

>[!NOTE]
>
>我们建议检查对象是否已按预期创建和连接。
