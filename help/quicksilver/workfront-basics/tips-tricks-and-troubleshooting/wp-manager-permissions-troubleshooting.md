---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Workfront校訂管理員許可權疑難排解
description: 中可用的許可權設定檔 [!DNL Adobe] 用於校訂使用者的Workfront為「管理員」、「主管」和「經理」。
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---

# [!UICONTROL [!DNL Workfront] 校訂管理員] 許可權疑難排解

以下為中可用的許可權設定檔 [!DNL Adobe Workfront] 校訂使用者：

* [!UICONTROL 管理员]
* [!UICONTROL 监督人]
* [!UICONTROL 经理]

<!--For detailed information about these options and how to configure them, see .-->

授與使用者時 [!UICONTROL 經理] 許可權，以下為可用的疑難排解資訊：

* **問題：** 使用者： [!UICONTROL 經理] 許可權無法檢視其他使用者建立的校樣。 相反地，他們看到 [!UICONTROL 存取遭拒] 畫面。

   ![](assets/access-denied-350x161.png)

   **解決方案：** 使用者： [!UICONTROL 經理] 必須將許可權明確新增至校樣。 校訂應一律透過 [!UICONTROL 進階校訂選項] 視窗和使用者應一律透過此選項新增。

* **問題：** 使用者： [!UICONTROL 經理] 許可權無法將校訂版本新增到其他使用者建立的校訂中（他們可能會在檔案集中提交校訂，但版本不會連線到其他使用者建立的原始集）。\
   **解決方案：** 使用者： [!UICONTROL 經理] 許可權只有在使用者具有以下許可權時，才能將版本提交給其他使用者的校訂 [!UICONTROL 經理] 許可權，條件為以下兩項：

   * 明確新增至校樣
   * 設定為 [!UICONTROL 作者] （校樣角色）在校樣上

* **問題：** 使用者： [!UICONTROL 經理] 許可權無法編輯其他使用者對他們未擁有或未建立之校訂的評論。\
   **解決方案：** 如果使用者具有 [!UICONTROL 經理] 許可權並不擁有校樣，但他們應該能夠編輯註解，並將它們新增為 [!UICONTROL 作者] (或 [!UICONTROL 版主])。\
   以下提供三種型別的許可權： [!DNL Workfront] 的 [!UICONTROL 計畫者]， [!UICONTROL 背景工作]， [!UICONTROL 請求者]， [!UICONTROL 檢閱者] 輸入授權。 中的系統管理員或使用者管理員 [!DNL Workfront] 可以編輯使用者的設定檔並調整 [!DNL Workfront Proof] 許可權。
