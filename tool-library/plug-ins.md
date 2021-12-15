# Wtyczki

Za pomocą narzędzia Plugin Manager zainstaluj przydatne wtyczki z od zespołu programu FormIt, lub dowiedz się, jak [**opracować własne wtyczki programu FormIt**](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)**.**

#### Narzędzie Plugin Manager programu FormIt

Narzędzie Plugin Manager programu FormIt działa jako centrum wyszukiwania wtyczek programu Formit i zarządzania nimi.

Narzędzie Plugin Manager jest wczytywane automatycznie podczas uruchamiania programu FormIt, o ile program FormIt ma dostęp do Internetu.

Dostęp do narzędzia Plugin Manager można uzyskać, klikając ikonę jego karty znajdującą się po prawej stronie okna aplikacji:

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PluginManagerTab.PNG)

#### Narzędzie Plugin Manager kategoryzuje różne typy wtyczek:

* **Zainstalowane wtyczki**
* **Zalecane wtyczki**
   * Wtyczki zalecane przez zespół programu FormIt na potrzeby rozszerzenia podstawowych funkcji programu FormIt i udostępnienia nowych procesów roboczych.
   * Po zatwierdzeniu przez zespół programu FormIt pojawią się tutaj wtyczki opracowane przez społeczność. W przyszłości zostanie udostępnionych więcej szczegółów na ten temat.
* **Wtyczki publiczne**
   * Wtyczki utworzone przez społeczność, które nie zostały zweryfikowane ani zatwierdzone przez zespół programu FormIt.

#### Narzędzie Plugin Manager zaprojektowano przy użyciu szeregu rozwijalnych i zwijanych interfejsów, co ułatwia zarządzanie wtyczkami i ich repozytoriami:

* **Zarządzanie wtyczkami:**
   * Kliknij nazwę wtyczki, aby zobaczyć jej opis.
   * Przełącz przełącznik, aby ją zainstalować lub odinstalować.
      * Wtyczka będzie widoczna jako pasek narzędzi w górnej części aplikacji, panel po prawej stronie lub okno dialogowe w środku, w zależności od jej typu.
* Jeśli [tworzysz własną wtyczkę](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html), możesz dodać jej prywatny adres URL w polu na dole i kliknąć \(+\):

![Narzędzie Plugin Manager programu FormIt](https://formit3d.github.io/FormItExamplePlugins/docs/images/addNew.png)

#### Jak działają wtyczki

* Wtyczki są oparte na technologii internetowej i są dostępne w programie FormIt dla systemu Windows oraz w wersji internetowej programu FormIt.
* Wtyczki składają się z serii plików i folderów przechowywanych w serwisie GitHub lub na serwerze lokalnym (w przypadku tworzenia własnej wtyczki).
* Wtyczki zewnętrzne \(wtyczki inne niż hostowane lokalnie\) wymagają połączenia z Internetem do wstępnego wczytania, co ma następujące konsekwencje:
   * Wtyczki zewnętrzne nie zostaną wczytane, jeśli podczas uruchamiania programu FormIt nie zostanie wykryte połączenie z Internetem.
   * Po wczytaniu niektóre wtyczki zewnętrzne mogą nadal działać w trybie offline w danej sesji, ale działanie innych może zostać przerwane, dopóki połączenie nie zostanie przywrócone.
   * Wtyczki zewnętrzne wczytują najnowszy kod na serwerze przy każdym uruchomieniu, więc ich funkcje są aktualizowane za każdym razem, gdy autor wprowadza zmiany.
* Wtyczki są wczytywane asynchronicznie, co oznacza, że kolejność wtyczek w interfejsie programu FormIt może się zmieniać podczas każdej nowej sesji.
* Narzędzie Plugin Manager używa kluczy rejestru w systemie Windows do przechowywania zainstalowanych repozytoriów i wtyczek.
   * Aby przywrócić domyślne ustawienia narzędzia Plugin Manager, należy usunąć następujący klucz rejestru:
      * Computer\HKEY\_CURRENT\_USER\Software\Autodesk\FormIt 360\Plugins
      * Należy pamiętać, że spowoduje to odinstalowanie wszystkich repozytoriów i wtyczek dodanych przez użytkownika, a więc zresetowanie narzędzia Plugin Manager do stanu, w którym będzie zawierać tylko wbudowane repozytoria i wtyczki.

