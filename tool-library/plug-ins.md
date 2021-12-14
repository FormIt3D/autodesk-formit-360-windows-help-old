# Moduly plug-in

Pomocí nástroje Plugin Manager nainstalujte užitečné moduly ze služby FormIt Team, nebo se naučte, jak[**vytvářet vlastní moduly plug-in aplikace FormIt**](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)**.**

#### Nástroj Plugin Manager aplikace FormIt

Nástroj Plugin Manager aplikace FormIt funguje jako centrum pro vyhledání a správu modulů plug-in pro aplikaci FormIt.

Nástroj Plugin Manager je načten automaticky při spuštění aplikace FormIt, pokud má aplikace FormIt přístup k internetu.

Nástroj Plugin Manager můžete otevřít kliknutím na jeho ikonu v pravé části okna aplikace:

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PluginManagerTab.PNG)

#### Nástroj Plugin Manager kategorizuje různé typy modulů plug-in:

* **Nainstalované moduly plug-in**
* **Doporučené moduly plug-in**
   * Moduly plug-in doporučované týmem aplikace FormIt. Tyto moduly rozšiřují základní funkce aplikace FormIt a odemykají nové pracovní postupy.
   * Moduly plug-in vyvinuté komunitou se zde objeví po schválení týmem aplikace FormIt. Podrobnější informace budou k dispozici v budoucnu.
* **Veřejné moduly plug-in**
   * Moduly plug-in vytvořené komunitou, které však nebyly přezkoumány ani schváleny týmem aplikace FormIt.

#### Nástroj Plugin Manager se skládá z řady rozbalitelných a sbalitelných rozhraní, což usnadňuje správu modulů plug-in a jejich úložišť:

* **Správa modulů plug-in:**
   * Kliknutím na název modulu plug-in zobrazíte jeho popis.
   * Přepnutím přepínače modul nainstalujete nebo odinstalujete.
      * V závislosti na typu modulu plug-in se modul zobrazí jako panel nástrojů v horní části aplikace, panel na pravé straně nebo jako dialog uprostřed aplikace.
* Pokud [vyvíjíte vlastní modul plug-in](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html), můžete přidat jeho soukromou adresu URL do pole v dolní části a kliknout na tlačítko \(+\):

![Nástroj Plugin Manager aplikace FormIt ](https://formit3d.github.io/FormItExamplePlugins/docs/images/addNew.png)

#### Jak moduly plug-in fungují

* Moduly plug-in jsou webové a jsou k dispozici v aplikaci FormIt pro systém Windows a FormIt pro web.
* Moduly plug-in se skládají z řady souborů a složek, které jsou uloženy na GitHubu (nebo na místním serveru, pokud si vytváříte vlastní).
* Externí moduly plug-in \(moduly plug-in, které nejsou hostovány místně\) vyžadují k počátečnímu načtení připojení k internetu, což znamená:
   * Externí moduly plug-in nebudou načteny, pokud při spuštění aplikace FormIt není zjištěno připojení k internetu.
   * Po načtení mohou některé externí moduly plug-in pro danou relaci pokračovat v práci v režimu offline, ale jiné se mohou přerušit, dokud nebude obnoveno připojení.
   * Externí moduly plug-in načítají nejnovější kód ze serveru při každém spuštění, takže jejich funkce se aktualizují vždy, když autor publikuje změnu.
* Moduly plug-in se načítají asynchronně, což znamená, že pořadí modulů plug-in v rozhraní aplikace FormIt se může v každé nové relaci měnit.
* Nástroj Plugin Manager používá v systému Windows k ukládání nainstalovaných úložišť a modulů plug-in klíče registru.
   * Pokud potřebujete obnovit výchozí nastavení nástroje Plugin Manager, odstraňte následující klíč registru:
      * Computer\HKEY\_CURRENT\_USER\Software\Autodesk\FormIt 360\Plugins
      * Upozorňujeme, že tímto způsobem odinstalujete všechny úložiště a moduly plug-in přidané uživatelem a obnovíte nástroj Plugin Manager tak, aby obsahoval pouze integrovaná úložiště a moduly plug-in.

