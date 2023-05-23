---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「篩選：顯示父系任務」
description: 您可以套用下面的任務篩選器以顯示工作任務。 工作任務是指可以獨立工作的任務，不是其他任務的父級任務。 在一個範例中，篩選器會識別可能是父系本身的子系任務。 在這種情況下，他們不是工作任務。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# 篩選：顯示父系任務

您可以套用下面的任務篩選器以顯示工作任務。 工作任務是指可以獨立工作的任務，不是其他任務的父級任務。 在一個範例中，篩選器會識別可能是父系本身的子系任務。 在這種情況下，他們不是工作任務。

>[!TIP]
>
>* 如果您考慮在報表中新增多個篩選器，建議您使用Report Builder介面新增所有篩選器，並在新增所有其他篩選器規則後按一下「切換至文字模式」 。 然後，您可以新增父系任務篩選器的程式碼，如上所述。 
* 我們也建議您為專案名稱新增分組，讓報告更易於閱讀。 如需有關將群組新增至報表的詳細資訊，請參閱文章 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>


## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>請求修改篩選器 </p>
   <p>計畫修改報告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改篩選器</p> <p><b>注释</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 顯示沒有子系的任務（可能有父系）

您可以將下列篩選器套用至任務報告，以顯示沒有子系的任務。 他們可以擁有自己的父母，也可以是其他工作的子女。

1. 從 **主要功能表** ![](assets/main-menu-icon.png)，按一下 **報表。**

1. 按一下 **新報告**.
1. 選取 **任務報告**.
1. 按一下 **篩選器**.
1. 按一下 **新增篩選規則**.
1. 在 **開始輸入欄位名稱……** 行，開始輸入 **子項數目**.

1. 選取 **等於（區分大小寫）** 若是您的修正因子，請輸入 **0** 的子項數目。\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   或

   按一下 **切換至文字模式**，並在文字編輯視窗中複製並貼上下列文字： 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. 按一下 **儲存+關閉**.

   這會為系統中正在執行任務的所有任務提取報告。 其中有些任務可能有父系任務，但它們本身並非父系任務。

## 與父項顯示任務（他們可能有子項）

您可以將下列篩選條件套用至任務報告，以顯示具有父系的任務，亦即它們是子系任務。 但是，這些任務也可能有自己的子項，因為篩選器未排除其子項。 同時作為其他任務父級的子任務不被視為工作任務。

1. 從 **主要功能表** ![](assets/main-menu-icon.png)，按一下**報表」。
1. 按一下 **新報告**.
1. 選取 **任務報告**.
1. 按一下 **篩選器**.
1. 按一下 **新增篩選規則**.
1. 在 **開始輸入欄位名稱……** 行，開始輸入 **父系ID**.
1. 選取 **不為空白** 為您的修飾元。

   ![](assets/filter-parent-id-not-blank-350x100.png)

   或

   按一下 **切換至文字模式**，並在文字編輯視窗中複製並貼上下列文字： 

   `parentID_Mod=notblank`

1. 按一下 **儲存+關閉**.

   這會為系統中具有父系且是這些父系的子系任務的所有任務提取報告。 其中部分工作本身可能是父系工作。

## 顯示沒有子系和父系的任務（獨立任務）

您可以將下列篩選器套用至任務報告，以顯示獨立的工作任務。 這些任務沒有父項，也沒有自己的子項。

1. 從 **主要功能表** ![](assets/main-menu-icon.png)，按一下 **報表。**
1. 按一下 **新報告**.
1. 選取 **任務報告**.
1. 按一下 **篩選器**.
1. 按一下 **新增篩選規則** 和 **開始輸入欄位名稱……** 行開始輸入 **子項數目** 選取 **等於（區分大小寫）** 若是您的修正因子，請輸入 **0** 的子項數目。
1. 按一下 **新增其他篩選規則** 和 **開始輸入欄位名稱……** 行開始輸入 **父系ID**，然後選取 **為空白**.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   或

   按一下「 」而非步驟6-7 **切換至文字模式** 在文字編輯視窗中，複製並貼上下列文字： 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. 按一下 **儲存+關閉**.

   這會為系統中沒有父項或子項的所有任務提取報告。 這些是獨立的工作任務。
