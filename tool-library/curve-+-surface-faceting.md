# Tvorba plošek křivek a povrchů

FormIt je polyhedralový modelovací systém, takže objekty jako kružnice, oblouky a křivky spline jsou reprezentovány řadou přímých hran. Podobně se zakřivená plocha, jako je stěna válce nebo kupole, skládá z řady rovinných ploch se skrytými hraničními hranami. 

Ve výchozím nastavení aplikace FormIt používá k reprezentaci kružnice 40 hran neboli plošek a 24 plošek k reprezentaci 3D zakřiveného objektu, jako je válec. U složitějších povrchů, jako je kupole, nastaví hodnota 24 počet plošek obvodu a také ovlivňuje hustotu plošek zbytku tvaru.

V aplikaci FormIt verze 18 a novější pro systém Windows si můžete hodnoty plošek křivek a povrchu přizpůsobit:

![](../.gitbook/assets/faceting\_planter.gif)

![](<../.gitbook/assets/faceting (1).png>)

**Kvalita tvorby plošek křivky**

Změna kvality tvorby plošek křivky ovlivní počet plošek použitých při kreslení nových kružnic a oblouků v aplikaci FormIt a také při umísťování základních tvarů. Například při nastavení na hodnotu 64 by se vytvořil 64stranný plný kruh nebo čtvrtkruhový oblouk se 16 ploškami.

Tato hodnota ovlivní také kvalitu kružnic a oblouků importovaných ze souborů SAT a také při zapékání geometrie z aplikace Dynamo. Tuto hodnotu můžete nastavit pro nové náčrty nebo pouze pro aktuální náčrt.

U existujících oblouků můžete také použít modul plug-in Rebuild Curve k retroaktivnímu novému vytvoření **existujícího** oblouku nebo kružnice s novým počtem plošek:

![](../.gitbook/assets/screen-shot-2020-01-10-at-1.20.53-pm.png)

![](../.gitbook/assets/faceting\_rebuild-curve.gif)

**Kvalita tvorby plošek povrchu**

Změna tohoto globálního nastavení ovlivní kvalitu 3D zakřivených povrchů importovaných ze souborů SAT a také při zapékání z aplikace Dynamo. 

Pokud například nastavíte hodnotu na 64 a poté z aplikace Dynamo zapečete kouli, bude použito 64 plošek kolem rovníku koule a 64 plošek v každé z kružnic směřujících k pólům koule, což se vše rychle sečte. Vyšší hodnoty používejte opatrně, protože v některých případech mohou ovlivnit výkon aplikace FormIt. Jakmile získáte výsledek ve vysoké kvalitě, můžete jej [převést na síť](meshes.md) a zlepšit tak výkon.

Při práci s aplikací Dynamo můžete upravit kvalitu tvorby plošek a kliknout na tlačítko „Run Graph“ na panelu vlastností, aniž byste měnili jakékoli parametry, což vám umožní snadno využít nové počty plošek:

![](../.gitbook/assets/faceting\_column.gif)

Stejně jako u křivek můžete nastavit kvalitu plošek povrchu pro nové náčrty nebo pouze pro aktuální náčrt.

Hodnoty plošek jsou v současné době omezeny na násobky 4, takže při ručním zadávání čísel bude aplikace FormIt zaokrouhlovat na nejbližší násobek. Přijatelné hodnoty můžete procházet pomocí posuvníků a šipek.

![](../.gitbook/assets/units-+-precision.png)
