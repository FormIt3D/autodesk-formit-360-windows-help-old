# Storefront/Curtainwall 豎框系統

![](../.gitbook/assets/dynamo-storefront-system-options.gif)

## 由 Dynamo 提供技術支援

這是 FormIt 中可快速建立店面/帷幕牆竪框系統的功能，由 Dynamo 提供技術支援。您可以在「Dynamo」面板中的「Dynamo Samples」目錄中找到 Storefront Curtainwall 系統：

![](../.gitbook/assets/storefront-curtainwall-button%20%281%29.png)

## 選取竪框系統的「玻璃」

從 FormIt 2021.2 開始，Storefront Curtainwall 系統使用新的 [SelectFromFormIt 節點](https://formit.autodesk.com/page/formit-dynamo#dynamo-formit-nodes)，可讓您選取要圍繞其產生竪框系統的「玻璃」\(單一面或擠出實體\)。

![一個簡單的玻璃平面，底部有門的開口。](../.gitbook/assets/storefron-system-1_glass-only.png)

按一下「Storefront Curtainwall」縮圖 \(請注意指出需要選取的圖示\) 時，FormIt 會提示您選取玻璃幾何圖形以繼續：

![](../.gitbook/assets/storefront-curtainwall-prompt.png)

有關選取玻璃如何運作的一些注意事項：

* 目前只支援平面表面。如果您選取一系列表面 \(例如，由許多較小平面表面組成的曲面\)，則腳本會尋找最大的平面，並使用該平面。
* 如果玻璃是實體 \(即單一面非常微小地擠出以表達一點厚度\)，則腳本會尋找最大的表面，讓產生的竪框會產生在玻璃實體的一側。
* 您可以繪製門的開口，並從玻璃邊界移除產生的表面，產生的竪框將遵循門開口，從而留出空間以加入門。
* 由於 Dynamo 的限制，如果玻璃幾何圖形中間有開口，則此腳本將無法運作。

## 秘訣與技巧

在 FormIt 中為 Dynamo 圖表選取幾何圖形時，某些組織技巧可簡化體驗並允許輕鬆引用結果：

* 將玻璃放在群組中，然後使用群組做為 Storefront/Curtainwall 腳本的選取。這樣，在產生竪框後，更容易編輯玻璃輪廓，如果在執行之間大量修改玻璃，且面 ID 發生變更，群組就可確保腳本永遠會找到玻璃，因為它使用的是群組 ID，而不是面 ID。
* 如果您打算將竪框系統的結果複製並貼到模型中的其他位置，最好將玻璃和產生的竪框包含在群組中。這也可避免選取節點在只複製並貼上產生的竪框群組時不知道要使用哪個玻璃實體的問題。
   * 先將玻璃放在群組中。按兩下以選取玻璃，然後按 G 或使用關聯式功能表或工具列中的「群組」指令。
   * 選取產生的群組，並將其放入其他群組。
   * 按兩下以輸入第一個群組。這是玻璃和產生的竪框的「容器」。
   * 按一下「Storefront Curtainwall」縮圖，然後使用「玻璃群組」做為選取。
   * 執行腳本後，您可以結束群組，並依需要複製/貼上容器。您可以編輯任何實體 \(調整玻璃形狀或參數\)，不會發生任何問題。

## 竪框系統選項

選取玻璃並執行腳本後，您會在 FormIt 圖元區中得到 FormIt 群組形式的結果。此群組將自動選取，且「性質」面板將顯示可用選項。

![](../.gitbook/assets/storefront-curtainwall-parameters.png)

* **執行**：如果您修改玻璃的造型並想要重新執行圖表以更新竪框結果，請按一下此按鈕。
* **編輯內嵌的圖表**：編輯產生幾何圖形的 Dynamo 腳本。此腳本內嵌在 FormIt 檔案中，只適用於此群組。
* **Select Glass \(Surface or Solid\)**：按一下此按鈕可將選取更新為要圍繞其產生竪框的不同玻璃片。

腳本將使用預設值執行第一次，因此您要針對您的獨特使用案例調整這些值。所有值將使用目前的 FormIt 單位。

* **Mullion Width + Depth \(豎框寬度 + 深度\)**：所有竪框元素的寬度和深度。
* **Vertical Mullion Spacing \(垂直豎框間距\)**：每根垂直竪框之間的中心距離。
* **Flip Vertical Mullion Layout \(翻轉垂直豎框配置\)**：腳本會從一側 \(任意選擇\) 開始垂直竪框間距。如果結果對於您的使用案例而言從錯誤的一側開始竪框間距，請將此設定為 True 翻轉配置，以從相反側開始。
* **Center Vertical mullion Layout \(中間垂直豎框配置\)**：不是在玻璃的一端開始計算垂直竪框間距，而是在中間開始計算，建立對稱的垂直竪框配置。
* **First Horizontal Mullion Spacing \(第一個水平豎框間距\)**：設定第一個水平竪框與底部的間距。如果您需要在底部放置一列較短的釉面玻璃模組，而且與其餘的水平竪框間距分開，此選項非常有用。
* **Horizontal Mullion Spacing \(水平豎框間距\)**：中心的典型水平竪框間距，從第一根竪框之後開始，如上所述。
* **Flip Horizontal Mullion Layout \(翻轉水平豎框配置\)**：如果您希望水平竪框配置從頂部而不是底部開始，請將此設定為 True。
* **Center Horizontal Mullion Layout \(中間水平豎框配置\)**：不是在玻璃底部或頂部開始計算水平竪框間距，而是在中間開始計算，建立對稱的水平竪框配置。

## 隱藏選項

尋找更多自訂？FormIt 的「性質」面板中隱藏了幾個進階選項，但可以按一下「編輯內嵌的圖表」，在 Dynamo 中顯示完整的圖表內容來存取這些進階選項：

![](../.gitbook/assets/dynamo-edit-embedded-graph.png)

### 隨機分隔竪框

![](../.gitbook/assets/storefront-curtainwall-random-verticals.png)

* **Randomize Vertical and Horizontal Mullion Layout \(隨機垂直與水平豎框配置\)**：將此設定為 True，可隨機分隔垂直或水平竪框
* **Min/Max Mullion Spacing \(if random\) \(最小/最大豎框間距，如果隨機\)**：調整這些值可設定最小和最大隨機間距值的範圍

### 邊界豎框

![](../.gitbook/assets/storefront-curtainwall-border-mullion-options.png)

* **Flip Offset Direction of Border Mullions \(翻轉邊界豎框的偏移方向\)**：竪框系統預設會使用玻璃邊界，並向內偏移以建立邊界竪框。若要向外偏移，請將此選項設定為 True。這會依「Mullion Width」設定增加竪框系統在玻璃邊界外部的整體大小。
* **Tolerance Between Selection and Border Mullions \(選取豎框與邊界豎框之間的公差\)**：竪框系統預設會在玻璃邊界處精確產生，這可能會導致在玻璃邊緣發生 Z-fighting 現象，且邊界竪框的外部表面發生碰撞。在大多數情況下不會看見此選項，但如果您的使用案例要求系統邊緣可見，而且您要避免 Z-fighting 現象，請啟用此選項並視需要調整公差值。

