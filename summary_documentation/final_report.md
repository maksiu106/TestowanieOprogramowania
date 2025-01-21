# Raport końcowy testowania systemu ewidencji herbaciarni Czajownia

### 1. Wprowadzenie

Poniższy raport zawiera podsumowanie wykonanych testów dla systemu ewidencji herbaciarni Czajownia w ramach przedmiotu Testowanie Oprogramowania odbywającego się na Wydziale Matematyki i Informatyki Uniwersytetu Jagiellońskiego w roku akademickim 2024/25. Oprogramowanie zostało zaprojektowane przez Michała Bargiela.

### 2. Szczegóły

- **data wykonania raportu**: 21.01.2024
- **tester**: Krzysztof Czarnowus

### 3. Cel i zakres testów

- **cel**: Szczegółowe zbadanie używanego od kilku lat systemu w kontekście wsparcia określenia wymagań przed dalszym rozwojem aplikacji bądź zaprojektowaniem nowej o analogicznym przeznaczeniu.
- **strategia**: Przyjęto czarnoskrzynkową metodę testowania na aplikacji uruchomionej w środowisku docelowym. Początkowo planowano uruchomienie systemu w odizolowanym środowisku testowym, jednak natrafiono na istotne trudności (patrz: dział "Zidentyfikowane problemy", podpunkt 8).
- **zakres**: Przetestowano wszystkie kluczowe funkcjonalności  związanych z tworzeniem i modyfikacją zamówień, ustawianiem ich parametrów, modyfikowaniem bazy danych z ofertą towarów, zarządzaniem rezerwacjami, zbieraniem dobowych danych o zamówieniach, możliwości działania na wielu urządzeniach jednocześnie. Przeprowadzono również analizę wymagań niefunkcjonalnych związanych z czasem odpowiedzi, bezpieczeństwem oraz niezawodnością systemu.

### 4. Podsumowanie wyników testów

- **liczba wykonanych przypadków testowych**: 38
- **liczba zaliczonych przypadków testowych**: 20
- **liczba znalezionych błędów**: 18
- **procent sukcesu testów**: 52.6%

### 5. Zidentyfikowane problemy

| nr | przypadki testowe | opis znalezionego problemu | propozycja rozwiązania |
|----|-------------------|----------------------------|------------------------|
| 1 | TC‑TEASHOP‑07‑01, TC‑TEASHOP‑07‑02, TC‑TEASHOP‑07‑03 | **Brak limitu wprowadzanych znaków** dla wszystkich obecnych w systemie pól tekstowych wyraźnie zmniejsza bezpieczeństwo testowanego oprogramowania. Zauważono gwałtowny spadek czasu odpowiedzi przy wprowadzeniu dużej ilości tekstu. Podejrzewa się ryzyko uszkodzenia bazy danych przy potencjalnym przeładowaniu pamięci. | Wprowadzić limit znaków w polach tekstowych ‑ wartość limitu powinna być zależna od specyfiki danego pola. |
| 2 | TC‑TEASHOP‑07‑03 | **Zawodność systemu**. Zaobserwowano losowe i powtarzające się wyłączanie się funkcjonalności tworzenia nowej rezerwacji. Awaria trwa krótki czas. | Brak pomysłów co do źródła defektu ‑ zalecane jest bliższe przyjrzenie się odpowiedniemu fragmentowi kodu. |
| 3 | TC‑TEASHOP‑08‑01 | **Utrata ważnych informacji** podczas manipulowania danymi ‑ przenoszenia zamówień do archiwum i przywracania ich. Niektóre ważne parametry, jak np. status opłacenia zamówienia, zostają utracone. | Dodać do wartości przechowywanych w bazie danych kluczowy parametr, jakim jest status opłacenia zamówienia. |
| 4 | TC‑TEASHOP‑12‑03, TC‑TEASHOP‑12‑04 | **Wielokrotne wykonywanie poleceń** przy natychmiastowym dwukrotnym kliknięciu w dane pole. W efekcie niektóre dane zostają wprowadzone w postaci zdublowanej. | Wprowadzić zabezpieczenia uniemożliwiające wysłanie kolejnego polecenia podczas przetwarzania poprzedniego lub sprawdzanie podczas wprowadzania danych, czy nie utworzono już identycznego wpisu. |
| 5 | TC‑TEASHOP‑09‑01 | **Brak funkcji wieloplatformowości**. Część systemu zawierająca istotne aktualne informacje, jak np. przyjęte zamówienia, przechowywany jest w pamięci podręcznej przeglądarki, co uniemożliwia wydajne korzystanie z systemu na dwóch urządzeniach jednocześnie. | Zmodyfikować system komunikacji z bazą danych ‑ manipulowanie danymi powinno rozpocząć się na etapie otwierania zamówień, a nie dopiero podczas ich zamykania. |
| 6 | TC‑TEASHOP‑11‑01 | **Brak komunikatu zwrotnego podczas wydłużonego czasu przetwarzania polecenia**. Jest to wyraźne utrudnienie dla osoby niezaznajomionej dobrze z systemem. Niektóre funkcjonalności wyświetlają komunikaty zwrotne, podczas gdy inne nie, co należałoby ujednolicić. | Wprowadzić komunikaty zwrotne podczas wykonywania tych poleceń, które ich nie mają. |
| 7 | TC‑TEASHOP‑12‑01 | **Przeładowanie poleceń i zawieszenie ich przetwarzania** w elementach interfejsu operujących na pamięci podręcznej, czyli przede wszystkim wprowadzaniu danych dotyczących otwartego zamówienia. | Zastosowanie propozycji rozwiązania problemu nr 5 może prawdopodobnie pomóc również w tym przypadku. |
| 8 | brak pokrycia przypadkiem testowym | **Niemożliwość uruchomienia systemu w środowisku testowym**. Oprogramowanie powstało kilka lat temu i trudności w ponownym postawieniu serwera za pomocą Dockera wynikają prawdopodobnie ze zbyt wielu niezgodności w wersjach używanych narzędzi i bibliotek. Starsze są niewspierane, podczas gdy zastosowanie nowszych wymagałoby istotnych modyfikacji kodu źródłowego programu. System działa jednak na zewnętrznym serwerze i testy wykonano właśnie w środowisku docelowym, rezygnując z wykonywania najbardziej inwazyjnych działań, aby zminimalizować ryzyko zniszczenia działającego oprogramowania. | Wprowadzenie odpowiednich modyfikacji w produkcie, w miarę możliwości minimalizując ryzyko powtórzenia się sytuacji z czasem. |

### 6. Ocena jakości produktu

System nadaje się do użytkowania, co potwierdza stosowanie go przez kilka ostatnich lat, zidentyfikowane problemy przekładają się jednak na **brak niezawodności**, **wysokie ryzyko wystąpienia awarii** oraz **brak zabezpieczeń** przed niektórymi próbami celowego uszkodzenia systemu.

Większość zidentyfikowanych problemów powiązana jest z wymaganiami niefunkcjonalnymi, jednak znaleziono również defekty dotyczące niepełnego wprowadzenia oczekiwanych funkcjonalności. Zalecany jest dalszy rozwój we wskazanych powyżej obszarach.

### 7. Wnioski i rekomendacje

Wykonane testy nie pokryły wszystkich elementów systemu. Przypuszcza się, że zidentyfikowane problemy mogą wystąpić w większej ilości fragmentów interfejsu. Podczas dalszego rozwoju oprogramowania zaleca się wykazanie uważności i wrażliwości na stosowanie analogicznych zabezpieczeń dla podobnych elementów ewidencji.

Można również jednoznacznie określić, że najpoważniejszym znalezionym defektem jest **problem z uruchomieniem systemu** na nowoczesnych urządzeniach i że jest to pierwsza i najbardziej podstawowa rzecz, którą należy się zająć.

### 8. Najważniejsze załączniki

- [Specyfikacja wymagań](../requirements_specification.pdf)
- [Plan testów](../TESTPLAN.md)
- [Opis niskopoziomowych wypadków testowych](../low_level_test_cases.md)
- [Raport z wykonania przypadków testowych](./low_level_tc_report.md)
