---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Workfront Proof Manager权限疑难解答
description: 以下是 [!DNL Adobe] Workfront（用于校对用户） — 编辑我。
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: ecb6928c946203b03a93cf5687fd53abf8e6a8f3
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 1%

---

# [!UICONTROL [!DNL Workfront] 校样管理器] 权限疑难解答

以下是 [!DNL Adobe Workfront] 对于校对用户：

* [!UICONTROL 管理员]
* [!UICONTROL 监督人]
* [!UICONTROL 经理]

<!--For detailed information about these options and how to configure them, see .-->

授予用户时 [!UICONTROL 经理] 权限，则提供以下故障诊断信息：

* **问题：** 具有 [!UICONTROL 经理] 权限无法查看其他用户创建的校样。 相反，他们会看到 [!UICONTROL 拒绝访问] 屏幕。

   ![](assets/access-denied-350x161.png)

   **解决方案：** 具有 [!UICONTROL 经理] 权限必须明确添加到校样中。 校样应始终通过 [!UICONTROL 高级校对选项] 窗口和用户。

* **问题：** 具有 [!UICONTROL 经理] 权限无法将校样版本添加到其他用户创建的校样中（他们可能会在文档集中提交校样，但这些版本不会连接到其他用户创建的原始集）。\
   **解决方案：** 具有 [!UICONTROL 经理] 仅当用户具有 [!UICONTROL 经理] 权限：

   * 明确添加到校样中
   * 设置为 [!UICONTROL 作者] （验证角色）

* **问题：** 具有 [!UICONTROL 经理] 权限无法编辑其他用户对其不拥有或未创建的校样的评论。\
   **解决方案：** 如果用户具有 [!UICONTROL 经理] 权限不拥有校样，但他们应该能够编辑评论，并将其添加为 [!UICONTROL 作者] (或 [!UICONTROL 审核者])。\
   以下三种类型的权限可在 [!DNL Workfront] 表示 [!UICONTROL 计划员], [!UICONTROL 工作人员], [!UICONTROL 请求者], [!UICONTROL 审阅人] 键入许可证。 中的系统管理员或用户管理员 [!DNL Workfront] 可以编辑用户的配置文件并调整 [!DNL Workfront Proof] 权限。
