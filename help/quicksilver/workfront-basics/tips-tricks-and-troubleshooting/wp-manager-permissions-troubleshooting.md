---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Workfront Proof Manager权限疑难解答
description: 在 [!DNL Adobe] Workfront中可用于验证用户的权限配置文件是“管理员”、“主管”和“经理”。
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# [!UICONTROL [!DNL Workfront]验证管理器]权限疑难解答

以下是[!DNL Adobe Workfront]中可用于验证用户的权限配置文件：

* [!UICONTROL 管理员]
* [!UICONTROL 主管]
* [!UICONTROL 经理]

<!--For detailed information about these options and how to configure them, see .-->

在授予用户[!UICONTROL 经理]权限时，以下故障诊断信息可用：

* **问题：**&#x200B;具有[!UICONTROL 经理]权限的用户无法查看其他用户创建的验证。 他们反而会看到[!UICONTROL 访问被拒绝]屏幕。

  ![](assets/access-denied-350x161.png)

  **解决方案：**&#x200B;具有[!UICONTROL 经理]权限的用户必须明确添加到验证中。 应始终通过[!UICONTROL 高级校对选项]窗口创建校对，并应始终通过此选项添加用户。

* **问题：**&#x200B;具有[!UICONTROL 经理]权限的用户无法将验证版本添加到其他用户创建的验证中（他们可能会在文档集中提交验证，但这些版本不会连接到其他用户创建的原始集）。\
   **解决方案：**&#x200B;具有[!UICONTROL 经理]权限的用户只有在同时具有[!UICONTROL 经理]权限的用户同时满足以下条件时，才能将版本提交到其他用户的验证：

   * 明确添加到验证
   * 在验证上设置为[!UICONTROL 作者] （验证角色）

* **问题：**&#x200B;具有[!UICONTROL 经理]权限的用户无法编辑其他用户对其不拥有或未创建的验证的评论。\
   **解决方案：**&#x200B;如果具有[!UICONTROL 经理]权限的用户不拥有验证，但他们应该能够编辑评论，请将其添加为[!UICONTROL 作者] （或[!UICONTROL 审查方]）。\
   在[!DNL Workfront]中为[!UICONTROL 规划者]、[!UICONTROL 工作人员]、[!UICONTROL 请求者]、[!UICONTROL 审阅者]类型许可证提供了这三种类型的权限。 [!DNL Workfront]中的系统管理员或用户管理员可以编辑用户的配置文件并从此处调整[!DNL Workfront Proof]权限。
