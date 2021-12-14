# Sítě

Počínaje verzí 17.0 nabízí aplikace FormIt nový typ geometrie: sítě.

Sítě jsou zjednodušené reprezentace standardních objektů aplikace FormIt a umožňují výrazně zlepšit výkon geometrie s vysokým počtem polygonů, jako je nábytek, nebo 3D stafáž, jako jsou lidé, stromy, automobily a značení. Sítě jsou také vhodné pro složitou geometrii DWG, která by jinak mohla ovlivnit výkon aplikace FormIt.

Objekty lze převést na sítě a sítě lze převést zpět na objekty bez ztráty dat. Některé typy souborů jsou automaticky importovány jako sítě, například OBJ, STL a DWG. Další informace o převodu mezi typy a dalších výhodách a omezeních sítí naleznete níže.

### Převod objektů na sítě

Na sítě lze převést libovolnou kombinaci vrcholů, hran, ploch nebo těles.

Jednoduše vyberte objekty a buď použijte klávesovou zkratku OM \(Objekty na sítě\), nebo klikněte pravým tlačítkem a v místní nabídce vyberte položku Objekty na sítě:

![](../.gitbook/assets/context-menu_object-to-mesh.PNG)

Po převodu objektů na sítě se v horní části obrazovky zobrazí potvrzovací zpráva:

![](../.gitbook/assets/success_object-to-mesh.PNG)

**Při převodu objektů na sítě platí:**

* Hrany, které byly vyhlazeny na objektech, zůstanou vyhlazené i ve výsledných sítích.
* Orientace materiálů na objektech zůstanou ve výsledných sítích nezměněny.
* Síť je vytvořena pro každý použitý materiál. Pokud například převedete jednu krychli vybarvenou 6 různými barvami, získáte 6 různých sítí.
   * Převodem zpět na objekt jednotlivé sítě uzavřete zpět do tělesa.
* Výběrem tělesa převedete a nahradíte celé těleso sítí, ale výběrem jednotlivých hran nebo vrcholů, které jsou vlastněny tělesem, vytvoříte novou síť nad existující geometrií, aniž byste ovlivnili původní těleso.
* Převodem sady hran nebo vrcholů se vytvoří jedna síť čar \(síť tvořená hranami\) nebo jedna bodová síť \(síť tvořená body\), což znamená, že nebudete moci vybrat jednotlivé hrany nebo vrcholy, jakmile budou sloučeny do jediné sítě. Pokud chcete upravit polohu jednoho prvku, převeďte je zpět na objekty.

**Převod seskupené geometrie na sítě:**

* Sítě jsou ještě výkonnější, pokud můžete převést celou skupinu a všechny její vnořené skupiny na sítě.
* Skupiny a jejich vnořené prvky lze převést na sítě pomocí modulu plug-in:
   * V pravé části aplikace vyhledejte ikonu nástroje Plugin Manager:
      * ![](../.gitbook/assets/plugin-manager_icon.PNG)
   * Vyhledejte modul plug-in Mesh + Unmesh All a zaškrtnutím políčka jej nainstalujte:
      * ![](../.gitbook/assets/plugin-manager_mesh-unmesh-all.PNG)
   * Modul plug-in Mesh + Unmesh All se načte. Jednoduše vyberte skupinu obsahující objekty, které chcete převést na sítě, a klikněte na tlačítko Mesh All.
      * ![](../.gitbook/assets/mesh-unmesh-all-plugin.PNG)
   * Při převodu vnořených objektů nebo sítí pomocí tohoto modulu plug-in se v horní části obrazovky zobrazí zpráva s informací, kolik skupin a instancí skupin bylo touto operací ovlivněno:

![](../.gitbook/assets/success_mesh-all.PNG)

### Interakce se sítěmi

**Vzhledem k jejich zjednodušené povaze mají sítě určitá omezení a chování:**

* Nebudete moci upravovat jednotlivé plochy, hrany ani vrcholy sítě.
   * Můžete však přebarvit sítě a přesouvat jednotlivé sítě vytvořené v důsledku použití různých materiálů na plochy \(viz výše\).
* Přichycení k sítím je omezeno na plochy a vrcholy sítí. Kvůli výkonu nebude přichytávání a odvozování fungovat s hranami sítí.
   * Soubory DWG převedené na sítě \(jiný typ sítě známý jako síť čar\) si však možnost přichytávání a odvozování s hranami sítí zachovají.
* U sítí nelze použít podlaží.
* Sítě nebudou hlásit problémy s vodotěsností ani se zadními plochami. Chcete-li zjistit, zda jsou vodotěsné, nebo ne, převeďte je zpět na objekty.
   * Objekty, které byly vodotěsné před převodem na síť, zůstanou vodotěsné i po převodu zpět na objekt.
* Sítě nelze použít v pokročilých operacích modelování, jako je připojení/oříznutí tělesa, 3D skořepina, 3D odsazení, zaoblení, šablonování, tažení nebo pokrytí.

Jinak se sítě zobrazují a chovají jako každý jiný objekt aplikace FormIt: lze je umístit ve skupinách, přiřadit k hladinám, vizualizovat ve scénách, používat pro analýzu atd.

**Interakci se sítí poznáte podle toho, že popisek nástroje zobrazí zprávu „On Mesh“ nebo že panel vlastností zobrazí informace o síti.**

![](../.gitbook/assets/snap_on-mesh.PNG)

![](../.gitbook/assets/properties-panel_mesh.PNG)

**Některé typy souborů jsou automaticky importovány jako sítě, aby se zvýšil výkon:**

* Soubory STL a OBJ, které mohou obsahovat hustou geometrii, například mračna bodů z jiných aplikací, se automaticky importují jako sítě.
* Soubory DWG, které mohou obsahovat miliony malých segmentů hran na vysoce kvalitních křivkách, se automaticky importují jako sítě.

### Převod sítí zpět na objekty

Jednoduše vyberte sítě a buď použijte klávesovou zkratku MO \(Sítě na objekty\), nebo klikněte pravým tlačítkem a v místní nabídce vyberte položku Sítě na objekty:

![](../.gitbook/assets/context-menu_mesh-to-object.PNG)

Po převedení sítí na objekty se v horní části obrazovky zobrazí potvrzovací zpráva:

![](../.gitbook/assets/success_mesh-to-object.PNG)

**Při převodu sítí zpět na objekty platí:**

* Všechny objekty, které byly před převodem na síť plné nebo vodotěsné, budou při převodu zpět na objekt znovu spojeny do vodotěsného tělesa.
* Převedením řady hran \(například ze souboru DWG\) nebo řady vrcholů \(například z mračna bodů\) na síť a zpět se objekty převedené ze sítě automaticky umístí do skupiny.
   * Tím se zabrání sloučení nových hran nebo vrcholů s jinou geometrií, což by mohlo mít nepříznivé účinky a dopad na výkon.
   * Pokud chcete hrany nebo vrcholy uvolnit, můžete jednoduše zrušit seskupení výsledné skupiny.

**Převod seskupených sítí zpět na objekty:**

* K převodu skupin a jejich vnořených sítí zpět na objekty použijte modul plug-in Mesh + Unmesh All a výše uvedené pokyny.

