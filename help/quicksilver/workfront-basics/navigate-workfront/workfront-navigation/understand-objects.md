---
content-type: overview;reference
navigation-topic: workfront-navigation
title: 瞭解中的物件 [!DNL Adobe Workfront]
description: 瞭解中的物件 [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '2263'
ht-degree: 6%

---

# 瞭解中的物件 [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

您在中顯示的資訊 [!DNL Adobe Workfront] 由儲存在 [!DNL Workfront] 資料庫。 物件是用來驅動資訊的 [!DNL Workfront].

瞭解在中如何定義物件 [!DNL Workfront] 非常重要，因此您可以使用正確的物件來滿足組織必要的需求。

例如，當您計畫大量工作時，您需要使用 [!UICONTROL 專案] 物件以定義該工作。 若要將此工作分成較小的計畫增量，您可以使用 [!UICONTROL 任務] 物件。 對於較少量未計畫且可能意外發生的工作量，您可以使用Issue物件。 如果您想要追蹤一組專案的進度與預算與時程表的遵守情況，您可以將其組織在 [!UICONTROL Portfolio] 和 [!UICONTROL 計畫]. 若要定義可協助您解決工作的其他元素，您想使用其他儲存在下的物件 [!UICONTROL 專案]， [!UICONTROL 任務]， [!UICONTROL 問題]，或 [!UICONTROL Portfolio]，按一下 [!UICONTROL 檔案]， [!UICONTROL 附註]， [!UICONTROL 小時]， [!UICONTROL 使用者]，或 [!UICONTROL 職位角色].

[!UICONTROL 報表] 和 [!UICONTROL 儀表板] 是另一個物件範例，可協助您整理資料量 [!DNL Workfront] 視覺化，方便所有使用者存取。

如需中物件的完整清單 [!DNL Workfront]，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

## 物件的相依性和階層

物件會在中彼此連結 [!UICONTROL Workfront]. 例如，任務或問題永遠不能獨立存在於專案之外。 [!UICONTROL 任務] 和 [!UICONTROL 問題] 是儲存在中的物件範例 [!UICONTROL 專案] 物件。 [!UICONTROL 任務] 和 [!UICONTROL 問題] 會視為專案的子物件。

以下是一些最常用的物件： [!DNL Workfront] 以及它們各自的父物件和子物件：

| **对象** | **父物件** | **子物件** |
|---|---|---|
| [!UICONTROL 项目组合] |  | [!UICONTROL 計畫]， [!UICONTROL 專案]， [!UICONTROL 檔案]， [!DNL Notes]， [!UICONTROL 使用者] |
| [!UICONTROL 项目群] | [!UICONTROL 项目组合] | [!UICONTROL 專案]， [!UICONTROL 檔案]， [!UICONTROL 附註]， [!UICONTROL 使用者] |
| [!UICONTROL 项目] | [!UICONTROL Portfolio]， [!UICONTROL 計畫] | [!UICONTROL 任務]， [!UICONTROL 問題]， [!UICONTROL 檔案]， [!UICONTROL 附註]， [!UICONTROL 小時]， [!UICONTROL 使用者] |
| [!UICONTROL 任务] | [!UICONTROL 项目] | [!UICONTROL 問題]， [!UICONTROL 子系任務]， [!UICONTROL 檔案]， [!UICONTROL 附註]， [!UICONTROL 小時]， [!UICONTROL 使用者] |
| [!UICONTROL 问题] | [!UICONTROL 任務]， [!UICONTROL 專案] | [!UICONTROL 檔案]， [!UICONTROL 附註]， [!UICONTROL 小時]， [!UICONTROL 使用者] |
| [!UICONTROL 仪表板] |  | [!UICONTROL 報表]，外部頁面 |
| [!UICONTROL 报告] | [!UICONTROL 仪表板] |  |
| [!UICONTROL 组] |  | [!UICONTROL 用户] |
| [!UICONTROL 团队] |  | [!UICONTROL 用户] |
| [!UICONTROL 用户] | [!UICONTROL 群組]， [!UICONTROL 團隊]， [!UICONTROL 公司] | [!UICONTROL 职位角色] |
| [!UICONTROL 公司] |  | [!UICONTROL 用户] |
| [!UICONTROL 文档] | [!UICONTROL 任務]， [!UICONTROL 問題]， [!UICONTROL 專案]， [!UICONTROL Portfolio]， [!UICONTROL 計畫]， [!UICONTROL 使用者] |  |
| [!UICONTROL 计划]* |  | [!UICONTROL 计划] |
| [!DNL Goals]* |  | [!UICONTROL 結果]， [!UICONTROL 活動] |

如需中物件的完整清單 [!DNL Workfront]，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

*計畫是 [!DNL Workfront Scenario Planner]. 如需關於以下專案的資訊： [!DNL Scenario Planner]，請參閱 [此 [!UICONTROL 案例規劃工具] 概觀](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL 目標] 物件屬於 [!DNL Workfront Goals]. 如需有關的資訊 [!DNL Workfront Goals]，請參閱 [[!DNL Adobe Workfront Goals] 概觀](../../../workfront-goals/goal-management/wf-goals-overview.md).


## 自訂物件名稱

As a [!DNL Workfront] 管理員，您可以自訂物件名稱 [!DNL Workfront] 透過使用  [!UICONTROL 版面配置範本].

如需有關如何使用自訂物件名稱的詳細資訊  [!UICONTROL 版面配置範本]，請參閱 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

自訂版面範本並將其指派給使用者後，這些使用者可以看到物件的自訂名稱。 已指派給版面配置範本的使用者不會再看到Web應用程式中任何位置的物件預設名稱。

>[!NOTE]
>
>使用者必須登出並重新登入，才能看到物件的新名稱 [!DNL Workfront] 在您儲存  [!UICONTROL 版面配置範本].

>[!IMPORTANT]
>
>此 [!DNL Workfront] 檔案一律參照物件的預設名稱。 As a [!DNL Workfront] 管理員，請務必通知使用者物件名稱的變更，以便他們瞭解如何使用 [!DNL Workfront] 檔案以及未反映物件名稱變更的應用程式區域。

* [可使用自訂的物件名稱  [!UICONTROL 版面配置範本]](#object-names-that-can-be-customized-using-a-layout-template)
* [區域 [!DNL Workfront] 反映自訂物件名稱的](#areas-of-workfront-that-reflect-the-customized-object-names)
* [區域 [!DNL Workfront] 未反映自訂物件名稱的物件](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### 可使用自訂的物件名稱 [!UICONTROL 版面配置範本]

As a [!DNL Workfront] 管理員，您可以自訂下列物件的名稱，以符合組織中的術語：

* [!UICONTROL 项目组合]
* [!UICONTROL 项目群]
* [!UICONTROL 项目]
* [!UICONTROL 任务]
* [!UICONTROL 问题]
* [!UICONTROL 目标]*
* [!UICONTROL 结果]*
* [!UICONTROL 活动]*

   *[!UICONTROL 目標]， [!UICONTROL 個結果]、和 [!UICONTROL 活動] 僅適用於貴公司已購買時 [!DNL Workfront Goals]. 如需有關的資訊 [!DNL Workfront Goals]，請參閱 [[!DNL Adobe Workfront Goals] 概觀](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL 计划]**
* [!UICONTROL 方案]**
* [!UICONTROL 计划]**

   **[!UICONTROL 行動方案]， [!UICONTROL 情境]、和 [!UICONTROL 計畫] 僅在貴公司購買 [!DNL Workfront Scenario Planner]. 如需關於以下專案的資訊： [!DNL Scenario Planner]，請參閱 [開始使用 [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).


例如，如果組織中較大量的工作稱為「參與」，您可以取代名稱「[!UICONTROL 專案]&#39;具有&#39;Engagement&#39;。 您的 [!DNL Workfront] 介面會顯示「參與」而非「[!UICONTROL 專案]&#39;只要有名稱&#39;[!UICONTROL 專案]「 」將會出現。

有關如何使用自訂物件名稱的詳細資訊  [!UICONTROL 版面配置範本]，請參閱 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

您無法在Workfront中自訂任何其他物件的名稱。 如需中物件的完整清單 [!DNL Workfront]，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

當您自訂物件的名稱時，該物件的新名稱會出現在的大部分割槽域中。 [!DNL Workfront] 顯示物件名稱的應用程式。

### 區域 [!DNL Workfront] 反映自訂物件名稱的

下列區域顯示物件的更新名稱：

* 顶端导航
* 左側面板導覽中的所有區段
* 所有功能表
* 應用程式內通知
* Report Builder和報告元素（檢視、篩選器和群組）
* [!UICONTROL 儲存] 按鈕
* 匯出的檔案
* 电子邮件
* 行動應用程式

### 區域 [!DNL Workfront] 未反映自訂物件名稱的物件

下列區域不顯示物件的更新名稱：

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] 增益集

## 自訂物件名稱的影響

自訂中的物件名稱時，請注意下列事項 [!DNL Workfront]：

* 您可能會在系統顯示中遇到文體或文法錯誤。 例如，如果您重新命名「[!UICONTROL 問題]&#39;變成&#39;Request&#39;，而您在系統中的任何地方看到&#39;An request&#39;這個片語都會如預期運作，不應該被視為錯誤。
* 您物件的自訂名稱無法翻譯。 僅限 [!DNL Workfront] 預設名稱可翻譯成支援的語言。 如需中支援語言的詳細資訊 [!DNL Workfront]，請參閱 [中支援的語言 [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). 自訂物件名稱欄位支援外來字元，因此您可以用任何語言輸入術語。
* 當您使用自訂物件名稱時  [!UICONTROL 版面配置範本]，建議您指派您的  [!UICONTROL 版面配置範本] 在您的業務單位（團隊或群組）周圍。\
   建議您使用這些業務單位的使用者清楚瞭解的名稱以避免混淆。
* 電子郵件通知和傳送的報表一律包含物件名稱，如以下所定義：  [!UICONTROL 版面配置範本] 產生電子郵件的使用者的。 如果您的使用者收到其他團隊和群組使用者的電子郵件通知，則使用者應準備好在其電子郵件中檢視與其群組或團隊無關的物件名稱。\
   As a [!DNL Workfront] 管理員，建議使用者注意與每個物件相關聯的圖示。 各物件名稱之間的圖示會保持一致，且與預設物件一致，如顯示在資料庫中的圖示一樣。 用於所有清單 [!DNL Workfront] 與物件相關聯的圖示，請參閱 [物件圖示](#object-icons).

   >[!TIP]
   >
   >對於組織中的常見工作，請考慮建立自訂檔案以反映您的術語。

## 物件圖示

此 [!DNL Workfront] 檔案一律參照物件的預設名稱。 如果您的物件已自訂其名稱，您可以依賴與其關聯的圖示來瞭解哪個自訂物件對應到哪個物件 [!DNL Workfront] 預設物件。

如需哪些物件可以有自訂名稱的詳細資訊，請參閱 [!DNL Workfront]，請參閱 [可使用自訂的物件名稱  [!UICONTROL 版面配置範本]](#object-names-that-can-be-customized-using-a-layout-template).

以下是Workfront中的物件及其對應圖示清單。

| **对象** | **图标** | **可自訂的物件名稱** |
|---|---|---|
| [!UICONTROL 公司] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL 仪表板] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL 目标] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL 组] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL 问题] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL 工作角色] | ![job_role_icon.png](assets/job-role-icon-52x50.png)， ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png)， ![](assets/job-role-nwe-no-color.png)， ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL 计划] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL 项目组合] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL 项目群] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL 项目] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL 报告] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL 任务] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL 团队] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL 模板] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## 物件的參考編號

在中建立的每個物件 [!DNL Workfront] 會指定一個唯一的參考編號。 參考編號可用來區分兩個在其他方面相似的物件（例如具有相同名稱的工作）。 您可以使用物件的參考編號來搜尋物件，也可以在報表中包含參考編號。

如需如何依參考編號搜尋物件的詳細資訊，請參閱 [使用物件的參考編號](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## 物件特定搜尋

您可以搜尋所有可搜尋的物件 [!DNL Workfront]，或者您可以選取要在基本和進階搜尋中搜尋的特定物件。

並非所有物件都可搜尋 [!DNL Workfront]. 您可以對下列物件執行基本和進階搜尋： [!DNL Workfront]：

| **对象** | **基本搜索** | **高级搜索** |
|---|---|---|
| [!UICONTROL 项目] | ✓ | ✓ |
| [!UICONTROL 任务] | ✓ | ✓ |
| [!UICONTROL 问题] | ✓ | ✓ |
| [!UICONTROL 报告] | ✓ | ✓ |
| [!UICONTROL 用户] | ✓ | ✓ |
| [!UICONTROL 模板] | ✓ | ✓ |
| [!UICONTROL 文档] | ✓ | ✓ |
| [!UICONTROL 项目组合] | ✓ | ✓ |
| [!UICONTROL 项目群] | ✓ | ✓ |
| [!UICONTROL 仪表板] | ✓ | ✓ |
| [!UICONTROL 公司] | ✓ | ✓ |
| [!UICONTROL 注释] | ✓ |  |

有關執行基本和進階搜尋的詳細資訊，請參閱： [!DNL Workfront]，請參閱 [搜尋 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## 物件報告

開始在中建立報表之前，瞭解物件的階層與相依性極為重要 [!DNL Workfront]. 報表是物件專屬的。 您必須先為報表選取正確的物件，才能顯示您想要的資料。

根據您為報表選取的物件，您只能存取直接連結至報表物件的物件。

>[!IMPORTANT]
>
>您只能報告您選取的物件以及相同報告中的父物件。 父物件報表中不能有子物件的相關資訊。 例如，您可以在任務報告中顯示專案資訊，但不能在專案報告中顯示任務資訊。

您可以使用我們的開放API來報告資料庫中的所有物件。 如需資料庫中所有物件的完整清單，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>如果您已使用版面配置範本自訂物件名稱，也會自訂Report Builder中的物件名稱。 確保您知道哪些物件已自訂，並在Report Builder中尋找自訂名稱。 如需哪些物件可以有自訂名稱的詳細資訊，請參閱 [!DNL Workfront]，請參閱 *[可使用自訂的物件名稱  [!UICONTROL 版面配置範本]](#object-names-that-can-be-customized-using-a-layout-template).*
>在報表中使用文字模式時，文字模式運算式中的物件名稱為中的標準名稱。 [!DNL Workfront]，而非自訂物件名稱。 如需在報表中使用文字模式的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

如需建立報表的詳細資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
如需API的詳細資訊，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

在中使用Report Builder時，您可以報告下列物件 [!DNL Workfront] 網頁應用程式：

* [!UICONTROL 项目]
* [!UICONTROL 任务]
* [!UICONTROL 小时]
* [!UICONTROL 问题]
* [!UICONTROL 用户]
* [!UICONTROL 访问级别]
* [!UICONTROL 审批]
* [!UICONTROL 批准流程]
* [!UICONTROL 分配]
* [!UICONTROL 待處理工作專案]\
   顯示敏捷待辦專案上的任務或問題。 如需有關敏捷待辦專案的詳細資訊，請參閱 [管理敏捷待處理專案](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

* [!UICONTROL 基线]
* [!UICONTROL 基线任务]
* [!UICONTROL 开票记录]
* [!UICONTROL 预算小时]

   這是 [!UICONTROL 預算時數]，如舊版已棄用的資源管理工具中所示。

   「Bud. 「小時」欄位 [!UICONTROL 已編列預算小時] 報告指標對工作角色預算的時數 [!UICONTROL 資源規劃工具]. 如需詳細資訊，請參閱 [瞭解 [!UICONTROL 預算勞力成本] 和 [!UICONTROL 預算時數] 適用於專案](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL 日历事件]
* [!UICONTROL 類別] (或 [!UICONTROL 自訂表單])
* [!UICONTROL 公司]
* [!UICONTROL 仪表板]
* [!UICONTROL 文档]
* [!UICONTROL 文档审批]
* [!UICONTROL 文档版本]\
   可讓您檢視檔案版本的各種相關資訊，包括檔案版本、版本相關聯的檔案、建立版本的使用者，以及在檔案版本上建立校樣的使用者（校樣建立者） （如果存在）。
* [!UICONTROL 电子邮件模板]
* [!UICONTROL 费用]
* [!UICONTROL 费用类型]
* [!UICONTROL 外部页面]
* [!UICONTROL 收藏夹]
* [!UICONTROL 筛选]
* [!UICONTROL 目标]

   您可以為策略目標建立報告，或當專案與目標關聯作為目標活動時，您可以在專案報告中顯示目標相關的資訊。 只有貴組織已購買，您才能建立策略目標並連線專案 [!DNL Workfront Goals] 授權。 如需有關的資訊 [!DNL Workfront Goals]，請參閱 [[!DNL Workfront Goals] 概觀](../../../workfront-goals/goal-management/wf-goals-overview.md). 如需將專案連結至策略目標的詳細資訊，請參閱 [在Adobe Workfront目標中新增專案](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: hardcoded links in this paragraph)
  </MadCap:conditionalText>
  -->

   >[!TIP]
   >
   >您無法報告與關聯的專案目標 [!UICONTROL 業務案例]. 如需有關專案目標與策略目標的資訊，請參閱 [字彙表 [!DNL Adobe Workfront] 術語](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL 组]
* [!UICONTROL 分组]
* [!UICONTROL 小时数类型]
* [!UICONTROL 计划]

   只有貴公司已購買，您才能為作為計畫子物件的計畫建立報告 [!DNL Workfront Scenario Planner] 授權。 如需方案的相關資訊，請參閱 [中的方案概觀 [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).


* 计划工作角色

   只有貴公司已購買，您才能為計畫中與行動方案相關的工作角色建立報告 [!DNL Workfront Scenario Planner] 授權。 如需建立方案並將其與工作角色建立關聯的資訊，請參閱 [在中建立和編輯方案 [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).


* [!UICONTROL 迭代]
* [!UICONTROL 工作角色]
* [!UICONTROL 日志条目]

   您可以在以下位置報告追蹤的系統更新： [!UICONTROL 更新] 任務、專案、問題等物件區域。 若要深入瞭解，請參閱 [報告 [!UICONTROL 更新] 區域](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL 布局模板]
* [!UICONTROL 里程碑]
* [!UICONTROL 里程碑路径]
* [!UICONTROL 注释]

   >[!NOTE]
   >
   >您可以報告個別使用者新增的註解。

* [!UICONTROL 引數] (或 [!UICONTROL 自訂欄位])
* [!UICONTROL 引數群組] (或 [!UICONTROL 分割槽符號])
* [!UICONTROL 入口網站設定檔] （這會顯示已棄用的資訊）
* [!UICONTROL 项目组合]
* [!UICONTROL 项目群]
* [!UICONTROL 專案] ([!UICONTROL 財務資料])

   >[!NOTE]
   >
   >財務資訊填入 [!UICONTROL 專案] ([!UICONTROL 財務資料])僅會在與其關聯的資料存在時間少於5年時報告。 例如，如果工作角色在2015年1月被分配給任務，而今天是2021年9月，則財務歸檔如下 [!UICONTROL 配置日期] （若為工作角色）不會填入 [!UICONTROL 專案（財務資料）] 報告。

* [!UICONTROL 校对审批]\
   可讓您檢視有關校訂核准的各種資訊，包括：已提交以供核准的校訂、關於以下專案的資訊： [!UICONTROL 核准者]，要求者的相關資訊（如果要求者是已授權的） [!DNL Workfront] 使用者)、版本資訊、校訂ID和校訂建立日期。\
   [!UICONTROL 校訂核准] 報表僅包含可在使用者的「我的工作」區域中使用的校訂，這些區域尚未做出決定。\
   校訂核准指派於 [!DNL Workfront] 如說明 [將使用者新增至校訂](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) 在 [在中共用校訂 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL 队列]
* [!UICONTROL 队列主题]
* [!UICONTROL 評等] (這會顯示工作角色 [!UICONTROL 收費率] information)
* [!UICONTROL 提醒通知]
* [!UICONTROL 报告]
* [!UICONTROL 资源池]
* [!UICONTROL 风险]
* [!UICONTROL 风险类型]
* [!UICONTROL 计划]
* [!UICONTROL 记分卡]
* [!UICONTROL 团队]
* [!UICONTROL 模板]
* [!UICONTROL 模板任务]
* [!UICONTROL 空闲时间]

   您可以根據使用者在其個人資料中的指示，報告使用者的休假。

* [!UICONTROL 时间表]
* [!UICONTROL 时间表配置文件]
* [!UICONTROL 主题组]
* [!UICONTROL 用户委托]

   您可以報告受委派在辦公室外執行其他人任務和問題的使用者。 此報表顯示不在辦公室的使用者以及在外出期間履行職責的使用者。

* [!UICONTROL 查看]
* [!UICONTROL 工作專案] （這指任務和問題）
