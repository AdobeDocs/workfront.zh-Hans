---
title: 檢視群組中配置及使用的授權數目
description: 身為Adobe Workfront管理員，您可以檢視目前用於群組及其子群組的個別授權型別計數。 當您需要評估是否要重新分配授權時，這個選項會很有用。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: 0e8f8973ad4c1310b973bae4e6fe3578c05db204
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 0%

---

# 檢視群組中配置及使用的授權數目

身為Adobe Workfront管理員，您可以檢視目前用於群組及其子群組的個別授權型別計數。 當您需要評估是否要重新分配授權時，這個選項會很有用。

如果您管理的群組上方有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

>[!IMPORTANT]
>
>只有當群組是使用者的「主群組」時，才會在特定群組中計算使用者的授權。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>计划 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完全管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要瞭解自己擁有的計畫或授權型別，請聯絡Workfront管理員。

## 檢視群組中使用的授權數量

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Adobe Workfront右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

1. 按一下群組名稱。
1. 在顯示的頁面上，於右上角附近的標頭區域中檢視 **使用中的授權** 區域以檢視 **計畫** 和 **工作** 目前使用的授權。

   如果您檢視的是頂層群組，而Workfront管理員為群組定義了每個授權型別的最大數量，這些數字也會顯示。 例如，在以下群組中，最多10個使用者可以擁有計畫授權，15個使用者可以擁有工作授權：

   ![](assets/licenses-used-allocated.png)

   如需Workfront管理員如何為群組定義最大分配授權數量的相關資訊，請參閱區段 [設定主群組的授權數量上限](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) 在文章中 [管理系統中的可用授權](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >如果您要檢視的群組是子群組，您只能檢視正在使用的授權數目，而不是為群組配置的授權數目上限。 這是因為Workfront管理員並未定義子群組的授權數量上限。
   >
   >![](assets/subgroup-used-licenses-only.png)

1. 如需群組目前使用的每種授權型別（包括「檢閱」和「請求」）的個別計數，請按一下下方文字區域 **使用中的授權：**

   ![](assets/click-text-to-see-more.png)

   顯示的方塊為所有四種Workfront授權型別提供相同的資訊：計畫、工作、稽核和請求。 在方塊底部，您可以看到此群組或其子群組的成員所使用的授權總數：

   ![](assets/more-license-info.png)

   對於「檢閱和請求」授權，「最大值」欄一律顯示「無限制」。
