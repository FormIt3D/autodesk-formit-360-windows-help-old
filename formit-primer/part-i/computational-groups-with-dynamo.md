# 1.10 - Dynamo 的計算群組

_在本章中，我們將利用_ [_**Dynamo**_](http://dynamobim.org/) _的運算能力，來放置和修改與 OOTB Dynamo 圖表範例相關的彈性群組。_

_如果您未完成上一節，請從_ _**FormIt Primer Part 1 Datasets**_ _下載並開啟_ _**1.10 - Computational Groups with Dynamo.axm**檔案。_

_您可以_ [_**在此處進一步了解**_](http://formit.autodesk.com/page/formit-dynamo) _FormIt 與 Dynamo 如何協同合作以進行計算設計工作流程。_

## **建立下方露台樓梯**

1 - 確保 **Lower Terrace、Main Building Floor** 和 **Plan Image** 圖層都已開啟，因為我們將在此處加入樓梯。

2 - 放置連結到其中一個 OOTB Dynamo 範例的樓梯群組：

1. 在選項板列中開啟**「Dynamo」選項板**。您應該會在**「Dynamo Samples」**目錄中看到一些內建的 Dynamo 物件
2. 按一下 **Stairs** Dynamo 範例，將其帶入模型空間。FormIt 將在幕後執行圖表，並從此圖表產生樓梯幾何圖形。
3. 將游標移到圖元區上，樓梯載入後，樓梯幾何圖形的殘影預覽現在會與滑鼠一起移動。將游標移到圖元區上靠近露台的位置，然後按一下以放置樓梯。按 **Esc** 以清除選取。請注意，放置樓梯後，**「性質」選項板**會自動開啟。

![](../../.gitbook/assets/0%20%2815%29.png)

_**注意事項：**_[_**您也可以連結包含 Dynamo 圖表的本端目錄**_](https://formit.autodesk.com/page/formit-dynamo#dynamo-getting-started)_，並執行您自己的本端 Dynamo 圖表，就像這些範例一樣。_

3 - 更新樓梯標註：

1. 選取樓梯群組後，修改**「性質」選項板**底部 Dynamo **輸入**區段下可用的輸入，以符合下圖所示。透過 Dynamo 腳本建立的大多數群組在選取後，會在性質中包含 Dynamo 區段。
   * Add Top Landing \(加入頂部平台\) = False
   * Add Middle Landing \(加入中間平台\) = False
   * Add Bottom Landing \(加入底部平台\) = False
   * Floor-to-Floor Height \(樓板與樓板之間的高度\) = 2.6
   * Stair Width \(樓梯寬度\) = 12
   * Riser Height \(豎板高度\) = 0.6
   * Tread Length \(踏板長度\) = 1.25
   * Tread Overlap \(踏板重疊\) = 0.25
   * Tread Thickness \(踏板厚度\) = 0.25
   * Height Between Middle Landings \(中間平台之間的高度\) = \(由於未建立中間平台，因此不相關\)
   * Middle Landing Length \(中間平台長度\) = \(由於未建立中間平台，因此不相關\)
   * Top/Bottom Landing Length \(頂部/底部平台長度\) = \(由於未建立任何平台，因此不相關\)
2. 按一下**「執行」**按鈕，以使用更新的輸入值重新執行 Dynamo 腳本。
3. 依需要移動群組，將樓梯放置在與 **Plan Image** 相應的正確位置。移動樓梯群組時，請小心不要變更其高程。請參閱前幾章，進一步了解移動模型元素時的技巧和技術。

![](../../.gitbook/assets/1%20%2811%29.png)

_**注意事項：**_ _**Floor-to-Floor Height**_ _輸入是樓梯總高度的近似值。_ _**Riser Height**_ _是實際定義樓梯高度的參數。在此範例中，我們將_ _**「Floor-to-Floor Height」**_ _設定為 2.6'，但最後的樓梯高度是 3.0' \(0.6' \(**Riser Height**\) x 5 \(竪板數目\)\)。由於地面與樓板平台頂部之間的跨距為 3'-2"，因此剩餘的 2" 包含在上方竪板中。_

## **建立主建築樓梯**

_在先前的步驟中，我們建立了一個沒有平台的樓梯。現在，我們將建立一個使用上方平台對齊_ _**Main Building Floor** 的樓梯。_

1 - 首先為我們剛剛建立的樓梯製作複本：

1. 選取既有樓梯，然後按一下 **Plan Image** 上任意位置以啟動移動指令。這會讓 FormIt 使用 **Plan Image** 的高程做為放置新複本的起始參考高度。按 **Ctrl** 以製作**快速複本**。
2. 將游標移到主建築靠近露台上方的位置。請注意，現在露台的頂面是新的參考平面。按一下以放置群組。

![](../../.gitbook/assets/2%20%289%29.png)

_**注意事項：**_ _由於_ _**Plan Image**_ _位於_ _**地平面樓層**_ _平面，因此_ _**移動工具**_ _將使用該平面做為其起點的參考。請注意上圖中的__**「在面上」**__工具提示，指示「Plan Image」面已選取為起始參考，__**Lower Terrace Floor**__ 的頂面已選取為結束參考。_

2 - 使用**設為唯一 \(MU\)** 工具，以便在我們變更此樓梯的 Dynamo 輸入時，它不會影響下方樓梯。依需要重新定位群組，使其接近其最終位置 - 我們稍後將對此進行微調。您可以切換 **Lower Terrace** 圖層可見性查看下方平面以協助定位，但同樣地，在移動新樓梯時，請小心不要變更其高程。

3 - 在**「性質」選項板**中，如下所示更新 **Dynamo 輸入**，並再次執行腳本。

* Add Top Landing \(加入頂部平台\) = True
* Floor-to-Floor Height \(樓板與樓板之間的高度\) = 2.333
* Riser Height \(豎板高度\) = 0.466
* Tread Length \(踏板長度\) = 1.5
* Top/Bottom Landing Length \(頂部/底部平台長度\) = 2.5

![](../../.gitbook/assets/3%20%281%29.jpeg)

_**注意事項：**_ _如果您將_ _**「Add Bottom Landing」**_ _設定為_ _**「True」**_ _，並重新執行腳本，則底部平台的頂面應與_ _**Lower Terrace Floor** 的頂面對齊。發生此情況的原因是 \(與先前的樓梯不同\)，我們調整了 __**Riser Height**__，讓 __**Floor-to-Floor Height**__ 符合所需的真實高度 \(2'-4"或 2.333'\)。_

2 - 再將群組重新定位至其最終位置。頂部平台應與 **Main Building Floor** 齊平。

3 - 完成樓梯前，請對樓梯加入 **Stone - Travertine** 材料以與樓板相符。若要進一步了解如何套用材料，請參閱先前的章節。

