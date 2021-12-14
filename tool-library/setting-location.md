# Umístění nastavení

Nastavení umístění projektu na světě je důležité pro přesnost modelu a následných analýz:

* Umístění slouží k importu satelitního snímku, který lze použít k trasování existujícího pozemku nebo budovy.
* Umístění slouží k importu 3D terénu, který lze použít k odkazování na topologická data pozemku.
* Umístění slouží k přesnému určení polohy slunce na obloze, což ovlivňuje výpočet stínů.
* Umístění slouží k zajištění přesných analytických výpočtů při provádění analýzy slunečního záření a energetické analýzy.

Pro přístup k dialogu Nastavit umístění a jeho službám musíte být přihlášeni pomocí účtu Autodesk.

### Začínáme s umístěním

* Otevřete dialog **Nastavit umístění** pomocí nástroje **Umístění** na panelu nástrojů nebo pomocí klávesové zkratky SL.

![](../.gitbook/assets/location-toolbar.png)

* Začněte zadávat umístění projektu do vyhledávacího pole v levém horním rohu okna _Nastavit umístění_.

![](../.gitbook/assets/location-step-1%20%281%29.png)

* Vyberte jednu z automaticky vyplňovaných možností umístění nebo stisknutím klávesy Enter vyberte první možnost.
* Vyhledané umístění se automaticky přiblíží.

### Nastavení pouze umístění vs. import satelitního obrázku a terénu

Po vyhledání umístění si můžete vybrat jednu ze dvou možností:

* **Nastavit pouze umístění**: Nastaví umístění v souboru bez importu satelitního snímku.
* **Importovat satelitní snímek a terén**: Nastaví umístění a také importuje satelitní snímek a terén s použitím úrovně přiblížení a rozsahu, které lze konfigurovat.

### Import satelitních snímků

* V pravé horní části okna **Nastavit umístění** klikněte na možnost **Importovat satelitní snímek a terén**.
* Ve středu okna se zobrazí náhled satelitního snímku a údaj o tom, kde se vzhledem ke snímku zobrazí počáteční bod aplikace FormIt.

![](../.gitbook/assets/location-step-2.png)

* Přetažením satelitního snímku v rámci čtverce upravte jeho polohu.
* Jakmile čtvercová oblast obsahuje požadovaný snímek, klikněte na tlačítko **Dokončit import**.
* Snímek bude importován ve správném měřítku se skutečným severem směrem nahoru a bude vystředěn na počátek kreslicí plochy aplikace FormIt. Průhlednost a pořadí vykreslování importovaného snímku můžete změnit tak, že na něj dvakrát kliknete a přejdete do [**palety Vlastnosti**](../formit-introduction/tool-bars.md).

![](../.gitbook/assets/location-step-3.png)

### Aktualizace satelitního snímku

Po prvním importu satelitního snímku můžete v okně Nastavit umístění upravit úroveň přiblížení nebo rozsah satelitního snímku.

* Znovu otevřete okno **Nastavit umístění** z panelu nástrojů, jak je popsáno výše.
* Klikněte na tlačítko **Importovat satelitní snímek a terén**
* Zobrazí se aktuální úroveň přiblížení a rozsah satelitního snímku, jak je znázorněno na kreslicí ploše aplikace FormIt.
* Nyní stačí upravit polohu nebo přiblížení a kliknout na tlačítko **Dokončit import**, stejně jako předtím.
* Po novém importu snímku na kreslicí plochu se snímek přesune do správného umístění vzhledem k původní poloze obrázku \(již nemusí být vystředěn v počátku\):

![](../.gitbook/assets/location-step-4.png)

### Import terénu

Nově se v aplikaci FormIt 2021.3 při importu satelitních snímků pomocí dialogu **Nastavit umístění** importuje také terén.

![](../.gitbook/assets/terrain-button_original.png)

Terén je při importu umístěn na hladině, která je ve výchozím nastavení vypnutá \(v případě, že jste začali modelovat, by model mohl být zakrytý terénem\).

Když budete připraveni zobrazit terén, zapněte hladinu Terén zaškrtnutím políčka:

![](../.gitbook/assets/terrain-layer%20%281%29.png)

![](../.gitbook/assets/terrain_solid.png)

### Práce s terénem

Terén bude umístěn do skupiny aplikace FormIt. Dvakrát klikněte na skupinu, abyste ji mohli upravit.

Uvnitř najdete dvě sítě: jednu pro strany a dolní část a jednu pro horní část.

Pokud chcete upravit terén, je nutné převést sítě na jeden objekt tělesa:

* Vyberte obě sítě.
* Klikněte pravým tlačítkem a vyberte možnost Sítě na objekty nebo použijte klávesovou zkratku MO.

![](../.gitbook/assets/terrain-mesh-context.png)

Při současném převodu obou sítí na objekt je aplikace FormIt může zkombinovat do tělesa, rozloženého objektu, který lze použít k operacím s tělesy, jako je booleovský řez.

Zde můžete pomocí kombinace možností [Horní pohled](orthographic-views.md) a [Ortografická kamera](orthographic-camera.md) trasovat hranice pozemku v horizontální rovině a poté tuto rovinu vysunout do objemu, který protíná terén. Použití průhledného [materiálu](materials.md) pomáhá zobrazit terén skrz ořezávané těleso:

![](../.gitbook/assets/terrain-cutter-before.png)

Použijte nástroj Oříznout geometrii a vyberte terén jako „těleso, do kterého má být proveden řez“, a objem řezání jako „těleso, které má být odebráno“.

![](../.gitbook/assets/terrain-cut-menu.png)

Výsledkem bude terén s odebraným tělesem a prázdným místem, kam můžete nakreslit nový pozemek a základy.

![](../.gitbook/assets/terrain-cutter-after.png)

Pomocí [hladin](layers.md) můžete těleso oříznutí skrýt nebo dokonce vytvořit kopie terénu s řezem a bez něj pro případ, že byste potřebovali odkazovat na původní terén nebo změnit tvar řezu před provedením operace řezu objemovým tělesem.

