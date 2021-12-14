# Správce vrácení zpět

Aplikace FormIt nabízí jedinečný systém Zpět/Znovu, který lze použít dvěma různými způsoby, a to buď pro jednotlivé skupiny, nebo chronologicky a globálně:

* Příkaz Zpět/Znovu při úpravách vnořené skupiny ovlivní pouze změny uvnitř této skupiny.
   * To znamená, že můžete provést změnu v této skupině, poté provést mnoho změn v jiných skupinách, vrátit se do původní skupiny a mít možnost vrátit zpět poslední změny provedené v této skupině, aniž by to ovlivnilo změny provedené nedávno jinde.
* Příkaz Zpět/Znovu provedený z hlavního náčrtu \(nikoli při úpravách skupiny\) funguje tradičním způsobem: vrácena zpět bude poslední změna provedená v **libovolné** skupině na základě chronologického pořadí.

Správce vrácení zpět zaznamenává každou změnu v každé skupině modelu aplikace FormIt, včetně změn provedených v hlavním náčrtu. Nabízí tak vizuální přehled o tom, které operace byly zrušeny v kterékoli skupině modelu.

![](../.gitbook/assets/undo-manager.png)

Správce vrácení zpět **tučně** označí aktuální stav a navíc zobrazí všechny operace před tímto stavem a všechny operace, které dříve existovaly, ale byly od té doby vráceny zpět.

Kliknutím pravým tlačítkem myši na požadovaný stav a výběrem možnosti Přejít na se můžete podle potřeby vrátit do daného stavu modelu.

Skupiny, které byly explicitně odstraněny nebo již neexistují v důsledku použití příkazu Zpět nebo Znovu, jsou zobrazeny jako \*Neaktivní\*. Tyto skupiny lze obnovit opakovaným použitím příkazů Zpět nebo Znovu v rámci nadřazené skupiny, dokud se neobnoví.

