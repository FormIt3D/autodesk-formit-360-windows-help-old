# Často kladené otázky

## O aplikaci FormIt

**Co jsou aplikace FormIt a FormIt Pro?**

FormIt je 3D modelovací, vizualizační, analytické a výpočetní prostředí pro tvorbu architektonických návrhů.

Aplikace FormIt zahrnuje:

* Robustní modul pro modelování těles s výkonnými nástroji a pracovními postupy optimalizovanými pro navrhování budov
* Vylepšenou vizualizaci prostředí pro ilustraci možností návrhu, včetně uložených stavů modelu pomocí scén
* Umístění, satelitní snímky a 3D terén využívající službu Bing Maps
* Materiály z knihovny materiálů Autodesk
* Nástroje pro uspořádání modelu a viditelnost, například skupiny, hladiny a scény
* Nástroje pro analýzu, včetně následujících:
   * Ověření vodotěsnosti a zadních ploch pro diagnostiku a opravu modelu tělesa
   * Slunce a stíny
   * Analýza slunečního záření
   * Energetická analýza
* Integrace produktů společnosti Autodesk:
   * BIM 360 Docs
   * Insight \(Energetická analýza\)
   * [Dynamo](https://formit.autodesk.com/page/formit-dynamo)
   * [Revit](https://formit.autodesk.com/page/formit-revit)
* Podpora formátů souborů:
   * Otevření/Import
      * AXM, DWG, FBX, SAT, STL, OBJ, WSM, SketchUp, obrázky
   * Export
      * AXM, FBX, OBJ, STL, SAT, DAE, DXF

Aplikace FormIt je k dispozici zdarma pro systém [iOS](https://itunes.apple.com/us/app/autodesk-formit-360/id575282599?mt=8) a [v prohlížeči](https://app.formit.autodesk.com/). K používání aplikace [FormIt pro systém Windows](https://formit.autodesk.com/page/download), nejvýkonnější a funkcemi nejvíce vybavené verze aplikace FormIt, je vyžadováno předplatné aplikace **FormIt Pro**. Předplatné aplikace **FormIt Pro** také umožňuje používat další funkce ve verzích pro iOS a web, jako je analýza slunečního záření a energetická analýza. Aplikace **FormIt Pro** je součástí sady [Autodesk AEC Collection](https://www.autodesk.cz/collections/architecture-engineering-construction/overview).

**Co se stalo s aplikací FormIt pro systém Android?**

Ve snaze zjednodušit nabídku produktů FormIt jsme museli učinit těžké rozhodnutí o ukončení aplikace pro systém Android. Pokud ji máte nainstalovanou, bude fungovat i nadále, ale již není dispozici v obchodu Google Play.

**Jak mohu získat aplikaci FormIt?**

Chcete-li používat verzi pro systém Windows, musíte mít přístup k aplikaci **FormIt Pro**, která je součástí předplatného sady [AEC Industry Collection](https://www.autodesk.cz/collections/architecture-engineering-construction/overview). Pokud již tedy používáte aplikaci Revit, je velká pravděpodobnost, že již máte přístup k aplikaci FormIt. Aplikaci [FormIt pro systém Windows si můžete stáhnout přímo z našich webových stránek](https://formit.autodesk.com/page/download) nebo z aplikace Autodesk Desktop App.

Kromě toho můžete zdarma spustit webovou verzi přímo z našeho webu: [http://formit.autodesk.com](http://formit.autodesk.com)

Verzi pro iOS lze zdarma stáhnout z obchodu Apple App Store \(pouze pro iPad\).

**Pokud jsem student nebo pedagog, mohu získat přístup k aplikaci FormIt Pro zdarma?**

Ano! Přístup k předplatnému FormIt Pro získáte prostřednictvím portálu [Autodesk Education Portal](https://www.autodesk.com/education/free-software/formit-pro).

**Jak se naučím aplikaci FormIt používat?**

Nejlepším místem, kde začít, je výukový program [Základy aplikace FormIt](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Building-the-Farnsworth-House.html).

Tento výukový program obsahuje více částí, od začátečnických \(vytvoření celého moderního domu\) až po pokročilejší \(pokročilá práce s aplikacemi Revit a Dynamo\).

Můžete také využít naši řadu webinářů FormIt Friday, která obsahuje přes 20 videí. Naleznete je na našem [kanálu na YouTube](https://www.youtube.com/playlist?list=PLqumTDi1CVHM7rCHJs83Yb2FyadmuQsiH).

## Práce s aplikací Revit

**Jak aplikace FormIt funguje s aplikací Revit?**

FormIt je samostatná aplikace pro 3D kreslení a tvorbu návrhů, ale vytváří data, která lze snadno převést do aplikace Revit [pomocí doplňku FormIt pro aplikaci Revit](https://formit.autodesk.com/page/formit-revit).

**Co se stane při importu do aplikace Revit?**

Počínaje verzí 2016 se aplikace Revit dodává s doplňkem pro práci s daty aplikace FormIt. Při importu souboru AXM aplikace FormIt do aplikace Revit tento doplněk zkontroluje každý objekt v souboru a znovu jej vytvoří v aplikaci Revit pomocí rozhraní API. Ve výchozím nastavení je vše v aplikaci FormIt zařazeno do kategorie Objem.

Doplněk FormIt Converter přebírá každý objemový objekt a vytváří v aplikaci Revit rodinu Objem pomocí [rozhraní API přímého tvaru](https://knowledge.autodesk.com/search-result/caas/CloudHelp/cloudhelp/2016/CSY/Revit-API/files/GUID-DF7B9D4A-5A8A-4E39-8721-B7782CBD7730-htm.html).

Přímý tvar je objekt, který nelze upravovat, používaný v pracovních postupech IFC. Ačkoliv jej nelze upravovat, má značnou výhodu v tom, že umožňuje přenášet komplexní textury materiálů mezi aplikacemi FormIt a Revit. [Zde naleznete výukový program](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Revit-Interop.html), který podrobněji vysvětluje pracovní postup převodu z aplikace FormIt do aplikace Revit.

**Může aplikace FormIt vytvářet stěny, podlahy a další systémové rodiny aplikace Revit?**

Ne přímo. Jak je uvedeno výše, každý objekt je ve výchozím nastavení nastaven na kategorii Objem. K vytvoření stěn, podlah a podobně. je nutné model importovat do aplikace Revit pomocí doplňku Converter a potom pomocí nativních nástrojů aplikace Revit vytvořit systémové rodiny ze základního objemového modelu.

**Může aplikace Revit odeslat data zpět do aplikace FormIt?**

Ano. Chcete-li importovat data zpět do aplikace FormIt, exportujte celý soubor Revit nebo nejlépe jeho _část_ do formátu souboru SAT. Obvykle není nutné odesílat do aplikace FormIt VŠECHNA data aplikace Revit. Místo toho vytvořte v aplikaci Revit filtrovaný pohled, který obsahuje pouze minimální data \(například podlahy a stěny\), a teprve potom je uložte do souboru SAT.

## Práce s jinými aplikacemi

**Proč je výchozí formát souboru .AXM?**

Oficiální interní kódový název aplikace FormIt byl XModeler, takže formát souboru, který jsme vytvořili, byl Autodesk X Modeler neboli zkráceně AXM.

**Jaké typy 3D formátů může aplikace FormIt importovat?**

* Windows: AXM, DWG, FBX, OBJ, SAT, SKP, STL
* Web: OBJ, STL
* iOS: OBJ, STL, SAT

**Jaké typy formátů může aplikace FormIt exportovat?**

* Windows: FBX, OBJ, SAT, STL, DAE, DXF
* Web: OBJ, SAT, STL
* iOS: OBJ

**Jak aplikace FormIt spolupracuje s aplikací Dynamo?**

[Přečtěte si, jak aplikace FormIt a Dynamo spolupracují](https://formit.autodesk.com/page/formit-dynamo) při vytváření pracovních postupů výpočetních návrhů.

**Jaké jsou výhody aplikace FormIt v porovnání s aplikací SketchUp?**

* Lepší [**spolupráce s aplikací Revit**](../tool-library/revit.md) ****
* [**Integrace pro aplikaci Dynamo**](../tool-library/dynamo.md) pro výpočetní návrhy
* Nativní nástroje pro [**analýzu slunečního záření**](../tool-library/solar-analysis.md) a [**energetickou analýzu**](../tool-library/energy-analysis.md) využívající aplikaci Autodesk Insight
* Robustnější jádro pro modelování těles, které umožňuje pokročilé modelování
* Nativní pokročilé nástroje pro modelování, například [**Tažení, Pokrýt, Šablonování**](../tool-library/cover-sweep-loft.md), Odsazení tělesa, Tělesa skořepiny, 3D přechod/zaoblení a [**Vyrovnat plochy**](../tool-library/flatten-face.md)
* Více viditelných [**rovin řezu** ](../tool-library/section-planes.md)
* Diagnostické nástroje, například [**zobrazení problémů s vodotěsností a zobrazení zadních ploch**](../tool-library/visual-styles.md)
* [**Export částí modelu**](../tool-library/export-data.md) na základě toho, co je vybráno nebo viditelné
* Nativní export ve formátech OBJ, SAT a STL

**Mohu použít klávesové zkratky aplikace SketchUp?**

Ano! Aplikace FormIt pro systém Windows obsahuje plně upravitelnou mapu klávesnice. Mnoho běžných klávesových zkratek aplikace SketchUp je k dispozici již ve výchozím nastavení, ale můžete si je upravit v nabídce Upravit &gt; Předvolby.

**Mohu použít své soubory DWG?**

Ano! Aplikace FormIt může importovat 2D a 3D soubory DWG.

## Časté dotazy týkající se podpory

**Jak získám podporu?**

Můžete kontaktovat svého prodejce produktů společnosti Autodesk nebo využít [fórum pro uživatele aplikace FormIt](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=en). Doporučujeme nejprve hledat, zda na váš problém již nebyl zadán jiný dotaz, a pokud nenaleznete žádnou odpověď, publikujte nové téma a tým aplikace FormIt vám odpoví.

**Co mám dělat, pokud se nemohu přihlásit?**

* Tento [příspěvek na fóru](https://forums.autodesk.com/t5/formit-forum/having-trouble-logging-into-formit-for-windows-try-these-steps/td-p/7179572?profile.language=en) popisuje běžné problémy s přihlášením.
* Pokud máte počítač s přepínatelným grafickým procesorem (GPU), je důležité zajistit, aby aplikace FormIt vždy využívala výkonnější GPU. Zde jsou pokyny pro grafické karty společnosti [AMD](https://community.amd.com/docs/DOC-1581#jive_content_id_Assigning_Applications_to_GPUs) a [NVIDIA](http://nvidia.custhelp.com/app/answers/detail/a_id/2615/kw/manage%203d%20settings/related/1).

**Co mám dělat, pokud se nezdaří energetická analýza aplikace Insight?**

Pokud energetická analýza aplikace Insight hlásí chybu nebo nevrací žádné výsledky, [podívejte se na naši stránku věnovanou energetické analýze aplikace Insight](https://formit.autodesk.com/page/formit-insight), kde najdete tipy pro řešení problémů.

