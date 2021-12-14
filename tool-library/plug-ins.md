# 外掛程式

使用 Plugin Manager 從 FormIt 團隊安裝有用的外掛程式，或了解如何[**建置您自己的 FormIt 外掛程式**](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)**。**

#### FormIt Plugin Manager

FormIt Plugin Manager 可做為中樞來探索和管理 Formit 外掛程式。

只要 FormIt 有網際網路的存取權，當 FormIt 啟動時，Plugin Manager 就會自動載入。

您可以按一下應用程式視窗右側的頁籤圖示，以存取 Plugin Manager：

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PluginManagerTab.PNG)

#### Plugin Manager 對不同類型的外掛程式進行分類：

* **安裝的外掛程式**
* **建議的外掛程式**
   * FormIt 團隊建議的外掛程式，可擴充 FormIt 的核心功能並解鎖新工作流程。
   * 社群開發的外掛程式被 FormIt 團隊核准後，將顯示在此處。未來將會有更多詳細資料。
* **公用外掛程式**
   * 由社群建置，但尚未被 FormIt 團隊審閱或核准的外掛程式。

#### Plugin Manager 使用一系列可展開和可收闔的介面設計，可輕鬆管理外掛程式及其儲存庫：

* **管理外掛程式：**
   * 按一下外掛程式名稱可查看其描述。
   * 切換開關可安裝或解除安裝。
      * 外掛程式將以工具列顯示在應用程式頂端、右側的面板或中間的對話方塊，取決於外掛程式類型而定。
* 如果您[開發自己的外掛程式](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)，可以將其私人 URL 加到底端的欄位，然後按一下「\(+\)」：

![FormIt Plugin Manager](https://formit3d.github.io/FormItExamplePlugins/docs/images/addNew.png)

#### 外掛程式的運作方式

* 外掛程式以網頁為基礎，在 Windows 版 FormIt 和網頁版 FormIt 中提供。
* 外掛程式由一系列裝載在 GitHub 的檔案和資料夾組成，或在您建置自己的外掛程式時，由本端伺服器上的檔案和資料夾組成。
* 外部的外掛程式 \(不在本端裝載的外掛程式\) 需要網際網路連線才能初始載入，這表示：
   * 如果 FormIt 啟動時未偵測到網際網路連線，則不會載入外部外掛程式。
   * 載入後，有些外部外掛程式可以繼續在該工作階段的離線模式下運作，但有些外掛程式可能會中斷，直到連線恢復。
   * 外部外掛程式在每次執行時會在伺服器上載入最新的程式碼，因此每當作者推動變更時，功能都會更新。
* 外掛程式並非同步載入，這表示外掛程式在 FormIt 介面中的順序可能會隨每個新工作階段而變更。
* Plugin Manager 使用 Windows 上的登錄機碼儲存您安裝的儲存庫和外掛程式。
   * 如果您需要將 Plugin Manager 重置為其預設值，請刪除以下登錄機碼：
      * Computer\HKEY\_CURRENT\_USER\Software\Autodesk\FormIt 360\Plugins
      * 請注意，這會解除安裝所有使用者加入的儲存庫和外掛程式，並將 Plugin Manager 重置為只僅包括內建的儲存庫和外掛程式。

