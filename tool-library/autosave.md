# Autozapis

Od wersji 17.3 program FormIt dla systemu Windows zawiera funkcję Autozapis, która umożliwia tworzenie kopii zapasowej modelu FormIt podczas pracy. Używając tego pliku kopii zapasowej, można odzyskać dane, gdy program FormIt zostanie zamknięty bez zapisania zmian.

### Włączanie i wyłączanie autozapisu

Znajdź opcje konfiguracji funkcji Autozapis, wybierając opcje Edycja &gt; Preferencje &gt; Autozapis.

![](../.gitbook/assets/20190613-autosave.png)

Funkcja Autozapis jest domyślnie włączona, ale można ją całkowicie wyłączyć przez usunięcie zaznaczenia pola wyboru.

Ustaw czas \(w minutach\), co jaki funkcja Autozapis będzie wykonywała kopię zapasową, wprowadzając wartość w polu liczbowym „Interwał autozapisu”.

Pamiętaj, że te preferencje są wprowadzane na poziomie aplikacji i nie zmieniają się podczas otwierania różnych plików.

### Działanie funkcji Autozapis

Włączona funkcja Autozapis sprawdza, czy w bieżącym pliku programu FormIt znajdują się niezapisane zmiany. Jeśli istnieją niezapisane zmiany, Autozapis tworzy kopię zapasową pliku co określony czas.

Pliki kopii zapasowych są przechowywane obok oryginalnego pliku i mają rozszerzenie `.axmb`.

Na przykład jeśli oryginalny plik programu FormIt jest przechowywany w lokalizacji `C:/Users/<user>/FormIt/MyProject.axm`, plik kopii zapasowej można znaleźć w lokalizacji `C:/Users/<user>/FormIt/MyProject.axmb`.

Jeśli rozpoczynasz nową sesję programu FormIt, nie otwierając istniejącego pliku, niezapisane zmiany można znaleźć w lokalizacji `C:/Users/<user>/Documents/Untitled.axmb`. Po zapisaniu nowego modelu w innej lokalizacji funkcja tworzenia kopii zapasowej zacznie dodawać niezapisane zmiany obok nowej lokalizacji, jak wspomniano powyżej.

Po zapisaniu zmian w oryginalnym pliku funkcja Autozapis automatycznie usuwa plik kopii zapasowej, ponieważ kopia zapasowa jest teraz starsza niż oryginalny plik. Jednak wprowadzanie kolejnych zmian w zapisanym pliku spowoduje ponowne rozpoczęcie wykonywania kopii zapasowych przez funkcję Autozapis w określonych odstępach czasu.

Jeśli plik roboczy zawiera niezapisane zmiany, ale wybierzesz zamknięcie programu FormIt i odrzucenie zmian, kopia zapasowa funkcji Autozapis zostanie usunięta. Jednak jeśli zamknięcie programu FormIt zostało wymuszone — przez wyłączenie komputera lub awarię aplikacji — plik kopii zapasowej funkcji Autozapis zostanie zachowany i będzie można użyć go później do odzyskania danych.

### Praca z włączonym autozapisem

Program FormIt minimalizuje potencjalny wpływ funkcji Autozapis na wydajność, wykonując kopię zapasową w ramach oddzielnego procesu. W przypadku plików o małych i średnich rozmiarach wykonywanie kopii zapasowej przez funkcję Autozapis powinno być niezauważalne. W przypadku bardzo dużych plików \(około 400 MB lub więcej\) można zauważyć zaledwie chwilową przerwę, gdy program FormIt kopiuje cały model i rozpoczyna wykonywanie kopii zapasowej w oddzielnym procesie.

Jeśli zastanawiasz się, czy funkcja Autozapis wykonuje w danej chwili kopię zapasową, możesz sprawdzić, czy na pasku stanu w lewym dolnym rogu aplikacji jest wyświetlany krótki komunikat „Automatyczne zapisywanie...”:

![](../.gitbook/assets/20190613-autosave-status-bar.png)

Jeśli pasek stanu jest wyłączony, możesz go włączyć, wybierając opcje Okno &gt; Pasek stanu lub używając skrótu HS.

### Odzyskiwanie danych za pomocą funkcji Autozapis

Podczas otwierania pliku programu FormIt z dostępną kopią zapasową program FormIt poinformuje o istnieniu pliku kopii zapasowej. Jak wspomniano powyżej, może to być spowodowane zamknięciem programu FormIt bez wybrania opcji zapisania zmian w tym projekcie podczas jego ostatniej edycji lub nieoczekiwanym zamknięciem programu FormIt.

![](../.gitbook/assets/20190613-autosave-notification.png)

Kliknięcie hiperłącza „Otworzyć?” spowoduje wczytanie pliku kopii zapasowej `.axmb`.

Aby otworzyć kopię zapasową, można również użyć poleceń Plik &gt; Otwórz i ręcznie wybrać plik `.axmb` z eksploratora plików.

Po otwarciu pliku kopii zapasowej przy następnym zapisywaniu program FormIt będzie wymagał wybrania innego pliku FormIt \(`.axm`\) do zastąpienia. Nie można zastępować plików kopii zapasowej programu FormIt \(`.axmb`\).



