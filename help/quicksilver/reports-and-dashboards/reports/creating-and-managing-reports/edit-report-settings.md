---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 編輯報告設定
description: 您可以編輯報表的設定，以定義對其他使用者的顯示方式，或使用者在執行報表之前可提示輸入哪種資訊。
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 6%

---

# 編輯報告設定

您可以編輯報表的設定，以定義對其他使用者的顯示方式，或使用者在執行報表之前可提示輸入哪種資訊。

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
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯對報告、儀表板、行事曆的存取權</p> <p>編輯篩選器、檢視、群組的存取權</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 操作步驟

1. 開始建立報告，方法是前往 **主要功能表** > **報表**，然後選取報表的物件。

   或

   開啟現有報表，然後按一下 **報表動作** > **編輯**.

1. 按一下 **報表設定** Report Builder的右上角。
1. 設定下列報表設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">报告标题</td> 
      <td>指定報表的標題。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>指定說明報表用途和使用的陳述式。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">使用此報告的存取許可權執行</td> 
      <td>選取您希望此報告在顯示給其他使用者時，使用哪個使用者的存取許可權。 如需以其他使用者的存取許可權執行報告的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">使用其他使用者的存取許可權執行並傳遞報告</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">報告載入時，顯示</td> 
      <td>選取報告載入時為所有使用者顯示的預設標籤。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">報告在儀表板上載入時，顯示……專案</td> 
      <td>指定報告在儀表板上載入時，為所有使用者顯示的專案數。 預設值為15個專案，專案數量上限為200個。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在詳細資訊標籤上顯示資源格線檢視</td> 
      <td> <p>（僅限使用者報表）選取此選項可在報表的「詳細資訊」標籤上顯示「資源格線」。</p> <p>注意：將「資源格線」檢視套用至使用者報表時，該報表只會顯示處於「目前」狀態的專案。 如果您想檢視處於任何其他狀態的專案，可以使用「全域導覽列」的「人員」區域中的「使用者使用率」標籤，並在此套用「資源格線檢視」。 <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在詳細資訊標籤上顯示特殊檢視</td> 
      <td>（僅限專案報告）指定使用者在詳細資訊標籤上存取此資訊時將會看到的檢視型別。 例如，您可以選取「里程碑」或「甘特圖」檢視。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">默认情况下在甘特图中显示此报告</td> 
      <td>（僅限專案報表與任務報表）選取此選項，可在使用者檢視此報表中的「詳細資訊」標籤時，自動啟用「甘特圖」檢視。<br>如需有關在專案報告和任務報告中檢視甘特圖的詳細資訊，請參閱文章中的「在專案清單甘特圖中檢視任務資訊」一節 <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">檢視甘特圖中的資訊 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许在报告中改变查看方式</td> 
      <td>選取此選項，可讓使用者在執行報告時變更檢視。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许在报告中改变小组</td> 
      <td>選取此選項可讓使用者在執行報告時變更群組。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许在报告中更改筛选</td> 
      <td>選取此選項，可讓使用者在執行報表時變更篩選器。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **報告提示** 以設定報表的任何提示。\
   如需有關在報表中新增提示的詳細資訊，請參閱文章 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 按一下&#x200B;**完成，** 然後按一下 **儲存+關閉**.

## 其他信息

另請參閱：

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [開始使用Adobe Workfront中的報告](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [使用Adobe Workfront內建報表](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
