# 3D Text

## 由 Dynamo 提供技術支援

在 FormIt 2021 和更高版本中，您可以產生和修改由 Dynamo 提供技術支援的 3D Text 物件。Dynamo 可就地編輯文字的字體、大小和其他性質，在需要編輯時無需重新產生和重新定位文字。

![](../.gitbook/assets/3d-text.gif)

## 放置 3D Text

![](../.gitbook/assets/3d-text-placement.gif)

* 移至 Windows 版 FormIt 中的 Dynamo 面板，確保您位於「Dynamo Samples」目錄中。
* 按一下「3D Text」範例。
* 將游標移至圖元區，您會看到 3D Text 出現在游標上。
   * 放置前，您可以將游標懸停在幾何圖形上，以不同方式定位 3D Text - 例如，在垂直表面上讓文字本身垂直對齊。您也可以按 Tab 在不同方位之間循環。
* 按一下以放置將在 FormIt 群組內產生的 3D Text。
* 放置後，「性質」面板將會出現，以顯示 3D Text 的可用選項。

## 就地重複

使用 Dynamo 產生 3D Text 的美妙之處在於，編輯它很容易，而且可將文字留在目前位置，以便快速重複。

選取 3D Text 群組後或編輯群組時，「性質」面板中會提供 3D Text 的選項。

一開始放置 3D Text 後，「性質」面板將自動顯示。您也可以選取「群組」並自行切換至「性質」，或按兩下「群組」以自動切換至「性質」面板。

![](../.gitbook/assets/3d-text-options.png)

### Text \(文字\)

輸入您希望 3D Text 幾何圖形顯示的文字。此欄位也可以預覽選取的字體和對正方式。按 Enter/Return 可換行。

### Font \(字體\)

選取 3D Text 的字體。此清單將顯示電腦上可用的字體，選取新字體會更新「Text」欄位。

請注意，某些字體具有比較複雜的幾何圖形，使用 Dynamo 可能需要花費較多時間才能產生。

### Justification \(對齊\)

這會移動文字，相對於群組的局部座標系原點對齊。

* 「Left \(靠左\)」可確保文字從群組原點開始，並向右展開。
* 「Center \(置中\)」可確保文字永遠在群組原點周圍置中。
* 「Right \(靠右\)」可確保文字在群組原點處結束。

![](../.gitbook/assets/3d-text-justification-combined.png)

### Text Size \(文字大小\)

![](../.gitbook/assets/3d-text-text-size.png)

文字的高度 (以目前 FormIt 單位表示)。

### Extrusion Depth \(擠出深度\)

文字的 3D 擠出量 (以目前 FormIt 單位表示)。3D Text 設計為實體，所以此值不能為零，但您可以讓它非常接近 0，文字擠出狀況就不會太明顯。

### Tracking \(字元間距\)

![](../.gitbook/assets/3d-text-tracking.png)

「Tracking」有助於調整特定字體中字母之間的預設間距。使用目前的 FormIt 單位，可以是正數或負數。例如，以英尺為單位，0.25 會在每個字母之間增加 3" 的間距。相反地，-0.25 會讓所有字母靠近 3"。

### Multi-Line Spacing \(多行間距\)

![](../.gitbook/assets/3d-text-multi-line.png)

如果「Text」欄位中有多行，則此值會控制每行文字之間的間距。使用目前的 FormIt 單位。

### Invert Text \(反轉文字\)

![](../.gitbook/assets/3d-text-inverted.png)

如果為 True，此選項將在文字周圍建立一個實體，並從中移除文字，產生「反轉」文字的結果 - 就像從材料中挖掉文字一樣。

### Inverted Text Border \(反轉文字邊界\)

![](../.gitbook/assets/3d-text-inverted-border.png)

只有當「Invert Text」為「True」時才適用。指定文字周圍用於從實體移除文字的邊框量。使用目前的 FormIt 單位。

### Curve Faceting Quality \(曲線刻面品質\)

字體的曲線會使用 3D Text 轉換為線段，所以此值會控制曲線刻面的細緻程度。

數值越小，刻面越粗糙 \(線段越長\)，數值越大，刻面越細緻 \(線段越短\)。此值會取代「偏好」中 FormIt 的「曲線刻面」和「曲面刻面」設定。

### 執行

編輯選項後，按一下「執行」按鈕以執行基礎的 Dynamo 圖表，並產生新結果。參數如果變更，此按鈕將變為藍色，您就會知道要按一下「執行」才能在最後的幾何圖形中看到更新。 

### 編輯內嵌的圖表

按一下此按鈕將啟動 Dynamo 圖表編輯器環境，您可以檢視和編輯基礎的 Dynamo 圖表，以快速變更參數並查看即時更新，或檢查/調整邏輯。這不是必要的動作，但有助於疑難排解或更快進行編輯。請參閱下方以了解更多資訊。

## 在 Dynamo 中加快重複作業

如果您重複使用 3D Text 選項，啟動 Dynamo 圖表編輯器可能會更快，這可讓您調整參數並即時查看變更。這也能讓您在出現問題時檢查圖表背後的邏輯。

![](../.gitbook/assets/3d-text-edit-embedded.png)

您可以按一下「性質」面板中的「編輯內嵌的圖表」按鈕，以啟動 Dynamo 圖表編輯器。

![](../.gitbook/assets/3d-text-edit-embedded-windows.png)

## 疑難排解

3D Text 在幕後使用 Dynamo，Dynamo 使用一個稱為 ASM 的塑型核心產生其幾何圖形，而該幾何圖形會再傳回 FormIt。

某些字體可能會建立「自身相交的曲線」，或其他有問題的幾何圖形，這會導致 ASM 發生錯誤。

如果您在嘗試執行 3D Text 時發生錯誤，或字母消失，則可以按一下「編輯內嵌的圖表」查看圖表的錯誤，以及可能發生失敗的位置。

某些字體也有已知問題，讓它們無法轉換為正確的幾何圖形。Bahnschrift 是其中一個範例。如果您遇到其他有問題的字體，請[在論壇告訴我們](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=zh-CN)。我們將盡力修正特定字體的問題。





