# Railing Along Path

## 由 Dynamo 提供技術支援

在 FormIt 2021 和更高版本中，您可以沿路徑產生扶手，並快速就地自訂結果。Railing Along Path 由 Dynamo 提供技術支援，這表示您可以輕鬆規劃產生的扶手以獲得您想要的結果，重新執行邏輯將就地更新幾何圖形。

![](../.gitbook/assets/railing-along-path.gif)

## 啟動 Railing Along Path

* 移至 Windows 版 FormIt 中的 Dynamo 面板，確保您位於「Dynamo Samples」目錄中
* 按一下「Railing Along Path」範例
* 在螢幕左側，您會看到「Select path for railing」的提示
   * 您應該只選取一系列相鄰邊，或選取只包含一系列邊的群組。
   * 選取路徑後，按一下「完成」按鈕，或按 Enter/Return。
* 「Dynamo」面板會指示其正在處理變更。完成後，您在 FormIt 群組中會有一個 Dynamo 產生的扶手，可供您修改 \(請參閱下方\)。

## 就地重複

執行 Railing Along Path 後，您會發現其結果已設定為預設值。這些功能可能適合您，但您可以大量自訂扶手以滿足您的需求。

當 Railing Along Path 執行時，它會建立包含結果的新群組，FormIt 會自動選取該群組並顯示該 Railing Along Path 實體可用的選項。

您永遠可以透過選取「群組」並切換至「性質」面板，或編輯將自動顯示「性質」的「群組」，返回 Railing Along Path 的性質。

![](../.gitbook/assets/railing-along-path-options.png)

### Railing Height \(扶手高度\)

扶手的整體高度。使用目前的 FormIt 單位。

### Post Spacing \(支柱間距\)

主要垂直支柱之間的間距。使用目前的 FormIt 單位。

### Add Posts at Path Vertices \(在路徑頂點加入支柱\)

如果為 **True**，將在所選路徑的每個頂點加入支柱，並在該點重置下一個支柱定位的計算。

例如，如果您選取了一系列 3 條邊，則會在兩個內部點各顯示一個支柱。如果頂點指示方向發生變更 \(例如上樓或轉角\)，此選項會很有用。

如果為 **False**，只會沿路徑從一端開始加入支柱，並沿路徑測量距離，同時忽略沿路徑的頂點。如果您選取了頂點不重要的弧、雲形線或圓，並且希望支柱間距忽略它們，此選項會很有用。

### Reverse Path Direction \(反轉路徑方向\)

計算支柱的位置時，所選路徑的方向將決定路徑的哪一端開始測量支柱間距。

如果支柱間距導致路徑不想要的一端有剩餘空間，您可以將此值變更為 **True** 以翻轉曲線，並在另一端開始測量支柱間距。

### Post Width + Depth \(支柱寬度 + 深度\)

矩形垂直支柱輪廓的大小 \(在平面圖中\)。使用目前的 FormIt 單位。

### Handrail Width + Height \(扶欄寬度 + 高度\)

矩形扶欄輪廓的大小 \(在剖面圖中\)。使用目前的 FormIt 單位。

### Baluster Orientation \(欄杆方位\)

如果為 True，欄杆會像繩索一樣水平配向。如果為 False，欄杆會垂直配向，屬於較傳統的美感。

### Baluster width + Depth \(欄杆寬度 + 深度\)

欄杆矩形輪廓的大小。使用目前的 FormIt 單位。

### Baluster Spacing \(欄杆間距\)

每根欄杆之間的空間量。使用目前的 FormIt 單位。

### Bottom Rail Start Height \(底部扶手起始高度\)

扶手底部與支撐欄杆的底部扶手之間的距離。使用目前的 FormIt 單位。

### 執行

編輯選項後，按一下「執行」按鈕以執行基礎的 Dynamo 圖表，並產生新結果。參數如果變更，此按鈕將變為藍色，您就會知道要按一下才能在最後的幾何圖形中看到更新。‌

### 編輯內嵌的圖表

按一下此按鈕將啟動 Dynamo 圖表編輯器環境，您可以檢視和編輯基礎的 Dynamo 圖表，以更快速變更參數並查看即時更新，或檢查/調整邏輯。

