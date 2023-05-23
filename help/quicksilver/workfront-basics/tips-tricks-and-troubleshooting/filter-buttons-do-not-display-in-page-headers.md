---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 篩選器按鈕未顯示在頁首中
description: 閱讀本文章，疑難排解頁面標頭中未顯示的篩選按鈕。
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# 篩選器按鈕未顯示在頁首中

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 授權</strong></td> 
   <td> <p>[！UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>[！UICONTROL系統管理員]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

下列篩選按鈕不會顯示在各自的區域中：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] 區域</strong></td> 
   <td><strong>篩選按鈕</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL專案] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL我所在的專案]</p> </li> 
     <li> <p>[！UICONTROL我擁有的專案]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[！UICONTROL時間表]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[！UICONTROL我的時程表核准]</span> </p> </li> 
     <li> <p><span>[！UICONTROL我的時程表]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 解決方案

中的篩選按鈕 [!UICONTROL 專案和時程表] 區域未顯示，因為對應的篩選器未包含在套用至使用者的版面配置範本中。 此 [!DNL Workfront] 管理員必須指派包含篩選器的配置範本。

>[!NOTE]
>
>有時候，篩選器會從 [!UICONTROL 清單控制項] 區域於 [!UICONTROL 設定]. 此 [!DNL Workfront] 管理員必須將其包含在此區域的清單中，才能在版面配置範本中使用。

1. 確認版面配置範本顯示下列篩選器：

   * [!UICONTROL 我參與的專案] 和 [!UICONTROL 我擁有的專案] 在 [!UICONTROL 專案] 區域
   * [!UICONTROL 我的時程表核准] 和 [!UICONTROL 我的時間表] 在 [!UICONTROL 時間表] 區域

   若要這麼做：

   1. 存取配置範本。
   1. 選取 **[!UICONTROL 清單]** 在 **[!UICONTROL 自訂使用者看到的內容]**.
   1. 選取 **[!UICONTROL 專案]** 或 **[!UICONTROL 時間表]** 在 **[!UICONTROL 選取要自訂的清單]**.
   1. 在 **[!UICONTROL 篩選]** 區段，確認 **[!UICONTROL 我參與的專案]**， **[!UICONTROL 我擁有的專案]** （適用於專案）和 **[!UICONTROL 我的時程表核准]** 和 **[!UICONTROL 我的時間表]** （適用於時程表）已選取。
   1. 单击&#x200B;**[!UICONTROL 保存]**。

   如需詳細資訊，請參閱 [使用版面配置範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. 將版面配置範本指派給正確的使用者、職位角色、團隊或群組。 如需詳細資訊，請參閱 [將使用者指派至版面配置範本](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
