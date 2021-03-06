---
title: 應用
url: /user-guide/applications/
---

*應用程序作為[企業版](https://redirect.sonarsource.com/editions/enterprise.html) and [更高版本](https://www.sonarsource.com/plans-and-pricing/)的一部分提供。*

## 使用應用（Application）

應用 是多個專案的集合專案。假設您有一組專案由於技術上的原因被拆分，但是它們共享一個生命週期；它們在開發過程中會有直接交流，並且會一起被發布。有了 應用，它們可以在 SonarQube 中被視為一個單獨的實體，具有統一的專案主頁、問題（Issue）列表、度量（Measures）空間，且最重要的：品質門檻（Quality Gate）。

### 應用（Application）vs. 專案集（Portfolio）

應用 和 專案集 都是專案的集合，但是它們的目標不相同，因此用不同的形式表示。專案集 被設計為非常高階的執行結果概要，該概要顯示了僅有些許相關的一組專案在質量方面的表現，以及走向為何。應用 使您可以將一組專案視為一個較大的整體專案。例如，由於 應用 中的所有專案都是一起發布的，因此如果其中一個專案不可發布，則所有專案都不可發布，並且 應用 的綜合  品質門檻 為您提供了所有專案中必須修正的內容的即時摘要，以便您發布這組專案。

## 應用（Application）設定

在全域 專案集（Portfolio）管理界面中可創建和編輯 應用： **管理（Administration）> 配置（Configuration）> 專案集（Portfolios）**。更多資訊，請參見 [設置專案集和應用](/project-administration/configuring-portfolios-and-applications/)。應用 必須先由具有全域管理權限的用戶建立，但是在設置後，可以將單個 應用 的管理委派給其他用戶。

### 增加 應用（Application）數據

每次對一個專案進行分析之後，應用 都會被自動重新計算。如果要立即（重新）計算，則擁有對應 應用 管理權限的用戶可以使用 應用 層級 **管理（Administration）> 編輯定義（Edit Definition）** 界面中的 **重新計算（Recompute）** 按鈕。全域 專案集 管理界面：**管理（Administration）> 配置（Configuration）> 專案集（Portfolios）** 使您能夠立即將所有 應用 和 專案集 排進重新計算之佇列。

## 應用（Application）和 分支（Branch）分析

分支可於 應用 中使用。它們使您可以統計 應用 中的所有 分支 的專案。

**注意:** 避免在 應用 中添加可能被刪除的分支，以防止 應用 狀態出現問題。

設置完 應用 後，擁有對應 應用 之管理權限的任何人都可以在 **管理（Administration）> 編輯定義（Edit Definition）** 界面中手動建立一個新 分支。也可以從全域的 **管理（Administration）> 配置（Configuration）> 專案集（Portfolios）** 界面中管理 分支。對於每個 應用 分支，您可以選擇應該包括哪個專案分支，或該專案是否應該在分支中顯示。
