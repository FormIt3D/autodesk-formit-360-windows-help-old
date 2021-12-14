# Uchopení a odvození

Chcete-li si usnadnit kreslení a modelování, používejte k přesnému vytvoření, umístění a úpravě geometrie body uchopení a odvození. Jakoukoli zvolenou osu můžete použít jako osu pro kreslení nebo provedení jiné akce, například vysunutí povrchu.

**Poznámka:** _Informace o tom, jak urychlit používání nástrojů softwaru, najdete v části_ [_Klávesové zkratky_](../appendix/keyboard-shortcuts.md)_._

## Uchopení

Při vytváření náčrtů a modelování vám může pomoci několik uchopení. Přichytání k objektům je automaticky povoleno a přichytit se můžete k následujícím prvkům:

|                                                                                                                                                                            |                                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------ |
| Vrcholy | ![](<../.gitbook/assets/inf3 (3) (2).png>) |
| Hrany. Při umístění kurzoru nad hranu se na koncích a ve středovém bodu zabrazí malé červené tečky. | ![](../.gitbook/assets/inf4.png) |
| Středové body hrany | ![](../.gitbook/assets/inf5.png) |
| Rovina plochy. Při umístění kurzoru nad plochu se v těžišti plochy zobrazí malý červený bod. To vám usnadní nalezení bodu, pokud k němu chcete provést přichycení. | ![](../.gitbook/assets/inf6.png) |
| Těžiště ploch | ![](../.gitbook/assets/inf7.png) |
| Pracovní rovina, pokud neprovedete přichycení k jinému prvku. | ![](../.gitbook/assets/inf8.png) |
| Středy kružnic nebo oblouků | ![](../.gitbook/assets/inf9.png) |
| Vrcholy sítě | ![](../.gitbook/assets/inf2.png) |
| Rovina plošky sítě. | ![](../.gitbook/assets/inf1.png) |

Chcete-li provést přichycení k osnově, je nutné v nabídce Nastavení povolit možnost **Přichytit k osnově (SG)**.

## Osy a body odvození

Automatický výběr bodů odvození je vždy povolen a pomůže vám omezit pohyb geometrie. Osy odvození se generují automaticky pomocí nástrojů nebo při umístění ukazatele myši nad hrany nebo body. Osy odvození jsou na obrazovce vždy nakresleny čárkovaně, abyste věděli, kde jsou, a mohli k nim snadno provést přichycení.

**Osa:** Geometrii lze posunovat podél osy X, Y nebo Z. Osa X je červená, osa Y je zelená a osa Z je modrá.

![](../.gitbook/assets/inf10.png)

**Uzamknutí osy:** Pohyb můžete uzamknout podél osy X, Y nebo Z. Když jste na ose odvození, podržte klávesu Shift a poté pohybem myši proveďte přichycení a odvození k jiným prvkům.

![](../.gitbook/assets/inf13.png)

**Rovnoběžné:** Geometrii můžete nakreslit nebo přesunout rovnoběžně s existujícími prvky. Kolmá odvození jsou fialová. Je třeba umístit kurzor na čáru, kterou chcete použít jako rovnoběžnou referenci.

![](../.gitbook/assets/inf14.png)

**Kolmé:** Můžete také nakreslit nebo přesunout geometrii kolmo k existujícím prvkům. Kolmá odvození jsou fialová. Je třeba umístit kurzor na čáru, kterou chcete použít jako kolmou referenci.

![](../.gitbook/assets/inf15.png)

**Prodloužení z bodu:** Pomocí odvození můžete také provést prodloužení z referenčního bodu. Přesuňte ukazatel myši nad bod, který chcete použít jako referenci, dokud se nezobrazí popisek nástroje, a poté použijte osu odvození, která vede z tohoto bodu.

![](../.gitbook/assets/inf16.png)

**Střed kružnice:** Chcete-li provést přichycení ke středu oblouku nebo kružnice, přesuňte ukazatel myši nad oblouk nebo kružnici. Uprostřed se zobrazí malá červená tečka, která zůstane viditelná po dobu asi 5 sekund poté, co kurzor z oblouku nebo kružnice přesunete pryč. Nyní přesuňte kurzor nad tuto červenou tečku a proveďte přichycení ke středu.

![](../.gitbook/assets/inf17.png)

**Skutečné středové body oblouků a spline:** Při umístění kurzoru nad kružnici, oblouk nebo spline se budete moci přichytit ke skutečnému středovému bodu. Tento bod a koncové body budou zobrazeny malou červenou tečkou. Při odvozování na oblouk se také přichytíte k vrcholům přímých hran, které představují oblouk.

![](../.gitbook/assets/inf18.png)

**Odstranění odvození:** Je možné, že kreslení vygeneruje větší počet odvození, což může vadit v umístění bodů, které se nemají k těmto odvozením přichytit. Pokud stisknete klávesy **Shift+mezerník**, budou všechna odvození smazána, kromě těch, které se nacházejí v posledním umístěném bodě.

![Před vymazáním odvození](../.gitbook/assets/inf19.png)

![Po vymazání odvození](../.gitbook/assets/inf20.png)
