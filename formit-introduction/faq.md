# 常見問題

## 關於 FormIt

**什麼是 FormIt 和 FormIt Pro？**

FormIt 是一個建築設計的 3D 塑型、視覺化、分析和計算環境。

FormIt 功能：

* 強大的實體塑型引擎，具備針對建築設計最佳化的強大工具和工作流程
* 增強的環境視覺化，可展示設計選項，包括使用場景儲存的模型狀態
* 使用 Bing 地圖的位置、衛星影像和 3D 地形
* Autodesk Material Library 中的材料
* 模型組織和可見性工具，例如群組、圖層和場景
* 分析工具，包括：
   * 實體模型診斷和修復的無縫和背面驗證
   * 日光與陰影
   * 日光分析
   * 能源分析
* Autodesk 產品整合：
   * BIM 360 Docs
   * Insight \(能源分析\)
   * [Dynamo](https://formit.autodesk.com/page/formit-dynamo)
   * [Revit](https://formit.autodesk.com/page/formit-revit)
* 檔案格式支援：
   * 開啟/匯入
      * AXM、DWG、FBX、SAT、STL、OBJ、WSM、SketchUp、影像
   * 匯出
      * AXM、FBX、OBJ、STL、SAT、DAE、DXF

FormIt 可在 [iOS](https://itunes.apple.com/us/app/autodesk-formit-360/id575282599?mt=8) 和[瀏覽器](https://app.formit.autodesk.com/) 中免費取得。需要 **FormIt Pro** 固定期限的使用授權，才能使用 [Windows 版 FormIt]( https://formit.autodesk.com/page/download)，這是功能最強大且功能最豐富的 FormIt 版本。**FormIt Pro** 固定期限的使用授權還可在 iOS 和網路上啟用其他功能，例如「日光和能源分析」。[Autodesk 工程建設軟體集](https://www.autodesk.com.tw/collections/architecture-engineering-construction/overview)中包含 **FormIt Pro**。

**Android 版 FormIt 發生了什麼事？**

為了簡化 FormIt 產品提供，我們不得不做出終止 Android 應用程式的艱難決定。如果您已安裝，它將繼續執行，但無法再從 Play 商店取得。

**如何取得 FormIt？**

若要執行 Windows 版本，您必須擁有 **FormIt Pro** 的存取權，這是我們[工程建設軟體集](https://www.autodesk.com.tw/collections/architecture-engineering-construction/overview)固定期限使用授權的一部分。因此，如果您的辦公室有 Revit，您很有可能已經有 FormIt 存取權！您可以[直接從我們的網站](https://formit.autodesk.com/page/download)或從 Autodesk 桌面應用程式下載 Windows 版 FormIt。

此外，您也可以直接從我們的網站免費執行網頁版本：[http://formit.autodesk.com](http://formit.autodesk.com)

您可以從 Apple App Store \(僅限 iPad) 免費下載 iOS 版本。

**如果我是學生或教師，是否可以免費存取 FormIt Pro？**

是！您可以透過 [Autodesk Education Portal](https://www.autodesk.com/education/free-software/formit-pro) 存取 FormIt Pro 固定期限的使用授權。

**如何學習 FormIt？**

最好的開始位置是 [FormIt 入門手冊自學課程](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Building-the-Farnsworth-House.html)。

入門手冊有多個部分，範圍從初學者 \(建立整棟現代房屋\) 到更進階的內容 \(以更進階的方式使用 Revit 和 Dynamo\)。

我們的 FormIt 星期五線上研討會系列也有 20 多個影片。您可以在我們的 [YouTube 頻道](https://www.youtube.com/playlist?list=PLqumTDi1CVHM7rCHJs83Yb2FyadmuQsiH) 上找到這些影片。

## 與 Revit 搭配運作

**FormIt 如何與 Revit 搭配運作？**

FormIt 是一個獨立的 3D 草圖繪製和設計應用程式，但是它會建立可[使用 Revit 的 FormIt 增益集](https://formit.autodesk.com/page/formit-revit)輕鬆轉換為 Revit 的資料。

**匯入至 Revit 時會發生什麼事？**

自 2016 年起，Revit 隨附一個用於處理 FormIt 資料的增益集。當您將 FormIt AXM 檔案匯入至 Revit 時，此增益集會查看檔案中的每個物件，然後使用 API 在 Revit 中重新建立。FormIt 中的所有項目預設都會分類為「量體」。

FormIt 轉換器會採用每個量體物件，並使用 [Direct Shape API](https://knowledge.autodesk.com/search-result/caas/CloudHelp/cloudhelp/2016/CHT/Revit-API/files/GUID-DF7B9D4A-5A8A-4E39-8721-B7782CBD7730-htm.html) 在 Revit 中建立量體族群。

DirectShape 是 IFC 工作流程中使用的不可編輯物件。雖然它無法編輯，但是具備在 FormIt 和 Revit 之間轉移完整材料材質的明顯優勢。[這裡有自學課程](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Revit-Interop.html)，其中更詳細地說明 FormIt 至 Revit 的工作流程。

**FormIt 可以建立牆、樓板和其他 Revit 系統族群嗎？**

不是直接建立。如上所述，每個物件均預設為「量體」品類。若要建立牆、樓板等等，您應使用轉換器增益集將模型匯入 Revit，然後使用原生的 Revit 工具，從基本量體模型建立系統族群。

**Revit 是否可以將資料傳回 FormIt？**

可以。若要將資料匯回 FormIt，請將 Revit 檔案的全部或_部分_ (最好) 匯出為 SAT 檔案格式。通常不需要將您所有的 Revit 資料傳送至 FormIt。而是先在 Revit 中建立一個篩選視圖，其中僅包含最少量的資料 \(例如，樓板和牆\)，然後再儲存為 SAT。

## 與其他應用程式搭配運作

**預設檔案格式為什麼是「.AXM」？**

FormIt 正式命名前的內部代號是 XModeler，因此我們建立的檔案格式是 Autodesk X Modeler，簡稱 AXM。

**FormIt 可匯入哪些 3D 格式？**

* Windows：AXM、DWG、FBX、OBJ、SAT、SKP、STL
* 網頁：OBJ、STL
* iOS：OBJ、STL、SAT

**FormIt 可以匯出哪些格式？**

* Windows：FBX、OBJ、SAT、STL、DAE、DXF
* 網頁：OBJ、SAT、STL
* iOS：OBJ

**FormIt 如何與 Dynamo 搭配運作？**

[了解 FormIt 與 Dynamo 如何搭配運作](https://formit.autodesk.com/page/formit-dynamo)，以建立計算設計工作流程。

**FormIt 與 SketchUp 相比如何？**

* [**與 Revit 的互動**](../tool-library/revit.md)更好
* 與 [**Dynamo 整合**](../tool-library/dynamo.md)用於計算設計
* 適用於[**日光分析**](../tool-library/solar-analysis.md)和[**能源分析**](../tool-library/energy-analysis.md) \(由 Autodesk Insight 提供\) 的原生工具
* 更強大的實體塑型核心，能進行進階的塑型作業
* 原生進階塑型工具，例如[**掃掠、覆蓋、斷面混成**](../tool-library/cover-sweep-loft.md)、偏移實體/為實體建立薄殼、3D 混成/圓角以及[**將面弄平**](../tool-library/flatten-face.md)
* 多個可見的[**剖面平面**](../tool-library/section-planes.md)
* 診斷工具，例如[**顯示防水問題和顯示背面**](../tool-library/visual-styles.md)
* 根據選取和/或可見的內容[**匯出模型片段**](../tool-library/export-data.md)
* 原生 OBJ、SAT 和 STL 匯出

**我可以使用 SketchUp 鍵盤快速鍵嗎？**

是！Windows 版 FormIt 有一套完全可編輯的鍵盤對應。預設已經有許多常用的 SketchUp 快速鍵，但您可以在「編輯」&gt;「偏好」功能表中編輯。

**我可以使用我的 DWG 檔案嗎？**

是！FormIt 會匯入 2D 和 3D DWG 檔案。

## 常見支援問題

**如何獲得支援？**

您可以洽詢 Autodesk 經銷商，或在 [FormIt 論壇](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=zh-CN)上與我們聯繫。最好先搜尋您發現的問題，如果還沒有答案，請張貼新主題，FormIt 團隊將會回覆。

**如果我無法登入，該怎麼做？**

* 這篇[論壇文章](https://forums.autodesk.com/t5/formit-forum/having-trouble-logging-into-formit-for-windows-try-these-steps/td-p/7179572?profile.language=zh-CN)涵蓋常見的登入問題
* 如果您的電腦有可切換的圖形處理器 \(GPU\)，請務必確保 FormIt 永遠使用較高效能的 GPU。以下是 [AMD](https://community.amd.com/docs/DOC-1581#jive_content_id_Assigning_Applications_to_GPUs) 和 [NVIDIA](http://nvidia.custhelp.com/app/answers/detail/a_id/2615/kw/manage%203d%20settings/related/1) 的指示

**如果 Insight 能源分析失敗，該怎麼做？**

如果 Insight 能源分析報告錯誤或無法傳回任何結果，請[查看 Insight 能源分析頁面](https://formit.autodesk.com/page/formit-insight)，以取得常見的疑難排解秘訣。

