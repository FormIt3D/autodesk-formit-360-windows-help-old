# 曲線 + 曲面刻面

FormIt 是一個多面體的塑型系統，因此圓、弧和雲形線等物件是由一系列直邊表示。同樣地，圓柱壁或圓頂的曲面是由一系列具有隱藏邊界邊的平物面組成。

FormIt 預設使用 40 條邊 (或刻面) 來表示一個圓，使用 24 個刻面來表示一個 3D 彎曲物件 (例如圓柱)。對於圓頂之類更複雜的表面，值 24 會設定周長刻面計數，也會影響造型其餘部分刻面的密度。

在 Windows 版 FormIt v18 及更高版本中，可自訂曲線和曲面刻面值：

![](../.gitbook/assets/faceting\_planter.gif)

![](<../.gitbook/assets/faceting (1).png>)

**Curve Faceting Quality (曲線刻面品質)**

變更「Curve Faceting Quality (曲線刻面品質)」將影響在 FormIt 中繪製新的圓和弧時，以及放置基本造型時使用的刻面數。例如，將此設定為 64 會建立一個 64 邊的圓，或有 16 個刻面的四分之一圓弧。

此值也會影響從 SAT 檔匯入的圓和弧的品質，以及從 Dynamo 製作幾何圖形時的品質。您可以為新草圖或只為目前的草圖設定此值。

對於既有曲線，您也可以使用 Rebuild Curve 外掛程式，使用新刻面計數以追溯方式重新建置**既有的**弧或圓：

![](../.gitbook/assets/screen-shot-2020-01-10-at-1.20.53-pm.png)

![](../.gitbook/assets/faceting\_rebuild-curve.gif)

**Surface Faceting Quality (曲面刻面品質)**

變更此整體設定將影響從 SAT 檔案匯入之 3D 曲面的品質，以及從 Dynamo 製作時的品質。

例如，將此設定為 64，則從 Dynamo 製作一個圓球將在圓球赤道周圍使用 64 個面，在圓球移向兩極的每個環加上 64 個刻面，很快速就會完成！請謹慎使用較高的值，因為在某些情況下，它可能會影響 FormIt 的效能。一旦您得到高品質的結果，您可以[將其轉換為網格](meshes.md)以提升效能。

使用 Dynamo 時，您可以修改刻面品質，並在「性質」面板中按一下「執行圖表」，而不變更任何參數，以利用新的刻面計數：

![](../.gitbook/assets/faceting\_column.gif)

和曲線一樣，您可以為新草圖或只為目前的草圖設定曲面刻面品質。

請注意，刻面值目前限制為 4 的倍數，因此當手動輸入數字時，FormIt 會捨入為最接近的倍數。您可以使用滑棒和箭頭來循環檢視接受的值。

![](../.gitbook/assets/units-+-precision.png)
