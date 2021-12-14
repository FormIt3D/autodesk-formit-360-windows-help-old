# Skupiny

Jedna z nejzákladnějších, ale nejdůležitějších technik pracovních postupů aplikace FormIt zahrnuje seskupování. Skupiny zabraňují spojení geometrie a umožňují nastavit vztahy nadřazenosti/podřazenosti mezi kopírovanými prvky tak, aby se při aktualizaci jednoho prvku aktualizovaly oba prvky. Další informace o skupinách naleznete [zde](../formit-primer/part-i/grouping-objects.md).

Skupiny lze vytvářet a upravovat dvěma způsoby: buď z místní nabídky vybrané skupiny, nebo z hlavního panelu nástrojů.

## Interakce se skupinami

Chcete-li **vytvořit skupinu**, vyberte prvky, které chcete seskupit, například hrany, plochy, tělesa nebo jiné skupiny, a klikněte pravým tlačítkem myši. V místní nabídce vyberte nástroj **Skupina \(G\)**. Importované obrázky a satelitní snímky nelze seskupit.

Chcete-li **vybrat skupinu**, jednou na ni klikněte. Všimněte si přerušovaných čar, které se zobrazí při výběru skupiny. Tyto čáry označují celkovou velikost skupiny.

Chcete-li **upravit skupinu**, dvakrát na ni klikněte. Spustí se režim úprav, ve kterém lze pouze zobrazit a přichytit prvky mimo aktuální skupinu, ale nelze je vybrat. Prvky mimo aktuální skupinu lze také skrýt klávesovou zkratkou **H**.

Můžete vytvořit **skupiny v rámci skupin**: tyto skupiny se nazývají **vnořené skupiny** a lze je vytvořit v režimu úprav skupiny. Chcete-li se ve vnořených skupinách přesunout o jednu úroveň výše, klikněte kamkoli mimo skupiny.

Jestliže chcete **ukončit režim úprav skupiny**, dvakrát klikněte kamkoli mimo skupinu.

Můžete **kopírovat skupinu** a vytvořit tak vztah mezi původní skupinou a její kopií. Pokud upravíte jakékoli zkopírované skupiny, stejné změny se projeví ve všech souvisejících skupinách.

Chcete-li **přerušit vztah mezi zkopírovanými skupinami**, vyberte skupinu nebo skupiny, které chcete oddělit, klikněte pravým tlačítkem myši a v místní nabídce vyberte položku **Vytvořit jedinečné**. Možnost Vytvořit jedinečné můžete také vybrat na panelu nástrojů Skupiny.

Chcete-li **vybrat všechny související skupiny**, přesuňte ukazatel myši na skupinu a stiskněte klávesu Tab. Až se zvýrazní všechny související skupiny, kliknutím na tyto skupiny je vyberte. Poté můžete provést požadovanou akci pro všechny skupiny najednou.

[**Strom skupin**](groups-tree.md) umožňuje zobrazit a spravovat všechny skupiny v projektu na jediném místě.

## Místní nabídka skupin a přístup k panelu nástrojů

## ![](../.gitbook/assets/grouptoolbar.png)

**Prvky skupiny**

Chcete-li vytvořit skupinu pomocí panelu nástrojů Skupiny, vyberte jeden nebo více prvků, klikněte na ikonu **Vytvořit skupinu** a poté vyberte ikonu **Dokončit**. Případně můžete vybrat možnost **Vytvořit skupinu** na panelu nástrojů Skupiny, poté vybrat prvky, které chcete seskupit, a kliknout na ikonu **Dokončit**.

Pokud chcete **upravit skupinu pomocí panelu nástrojů Skupiny**, vyberte ikonu **Upravit skupinu** a poté klikněte na skupinu, kterou chcete upravit. Po dokončení úprav klikněte na ikonu **Dokončit**. Tento nástroj umožňuje vybrat k úpravám konkrétní skupinu, i když je hluboce vnořená.

**Chcete-li skupinu nastavit jako jedinečnou pomocí panelu nástrojů**, vyberte na panelu nástrojů Skupiny ikonu **Vytvořit jedinečné**. Můžete také na panelu nástrojů Skupiny vybrat možnost **Vytvořit jedinečné**, poté vybrat skupinu, kterou chcete nastavit jako jedinečnou, a kliknout na ikonu **Dokončit**.

**Chcete-li zrušit seskupení skupiny pomocí panelu nástrojů Skupiny**, vyberte skupinu, kterou chcete změnit, a v nabídce panelu nástrojů Skupiny vyberte ikonu **Zrušit seskupení**. Tím zrušíte seskupení aktuálního výběru, ale nezrušíte seskupení vnořených skupin. Případně můžete na panelu nástrojů vybrat možnost **Zrušit seskupení**, vybrat skupinu, kterou chcete změnit, a poté vybrat ikonu **Dokončit**.

**Chcete-li zrušit seskupení všech skupin vnořených pod aktuálně vybranou skupinou**, vyberte skupinu s vnořenými skupinami a na panelu nástrojů Skupiny vyberte možnost **Zrušit seskupení všech vnořených**.

**Chcete-li zrušit seskupení všech skupin v modelu**, vyberte na panelu nástrojů Skupiny možnost **Zrušit seskupení všeho**.

## Skupiny a aplikace Revit

Pokud jste obeznámeni s **rodinami** aplikace Revit, jste obeznámeni s koncepcí skupin v aplikaci FormIt. Skupiny aplikace FormIt mají funkce, které lze použít k jejich inteligentnímu přenosu do aplikace Revit.

**Kategorie skupin aplikace FormIt**

V aplikaci FormIt můžete zadat **kategorie** skupin tak, aby se z vašich skupin aplikace FormIt při importu do aplikace Revit staly rodiny stejných kategorií. Ke skupinám aplikace FormIt můžete přiřadit kategorie tak, že vyberete skupinu, přejdete do režimu **úprav skupiny** a pomocí panelu **Vlastnosti** vyberete požadované kategorie. Kategorie můžete také přiřadit na panelu **Strom skupin**.

**Názvy skupin aplikace FormIt**

K zadání názvu skupiny aplikace FormIt můžete použít také panel **Vlastnosti**. To může být užitečné při navigaci ve vlastním modelu a při importu modelu do aplikace Revit můžete prvky snadno filtrovat pomocí názvu skupiny.

Všimněte si, že **vnořené skupiny v aplikaci FormIt nejsou importovány do aplikace Revit jako vnořené skupiny**. Tím se zabrání hluboce vnořeným rodinám aplikace Revit.

