# Plan testów ewidencji herbaciarni Czajownia

## 1. Identyfikator planu testów

TP-TEASHOP-01

## 2. Wprowadzenie

Niniejszy plan testów ma na celu określić zakres, techniki oraz harmonogram testowania ewidencji herbaciarni Czajownia w ramach przedmiotu Testowanie Oprogramowania odbywającego się na Wydziale Matematyki i Informatyki Uniwersytetu Jagiellońskiego w roku akademickim 2024/25. Badane będzie spełnianie wymagań kluczowych do zapewnienia niezawodnego funkcjonowania systemu zarządzania zamówieniami oraz rezerwacjami, zarówno funkcjonalnych, jak i niefunkcjonalnych.

## 3. Testowana aplikacja

System POS (Point of sale) zaprojektowany przez Michała Bargiela dla herbaciarni Czajownia Kraków

## 4. Testowane funkcjonalności

Planowane jest przetestowanie wszystkich kluczowych funkcjonalności systemu: związanych z tworzeniem i modyfikacją zamówień, ustawianiem ich parametrów, modyfikowaniem bazy danych z ofertą towarów, zarządzaniem rezerwacjami, zbieraniem dobowych danych o zamówieniach, możliwości działania na wielu urządzeniach jednocześnie. Dodatkowo przeprowadzana będzie analiza wymagań niefunkcjonalnych związanych z czasem odpowiedzi, bezpieczeństwem, niezawodności oraz zgodności ze standardami systemów POS.

## 5. Funkcjonalności pominięte w testach

Testy nie obejmują modułów aplikacji działających w izolacji od całego systemu.

## 6. Podejście

Większość testów będzie przeprowadzana ręcznie przez testera bądź osoby zewnętrzne pod jego okiem. Część testów związanych z niezawodnością i czasem odpowiedzi zostanie wykonana przy pomocy wybranego później programu automatyzującego kliknięcia w odpowiednie miejsca ekranu.

Planowane jest wykorzystanie przede wszystkim podejścia czarnoskrzynkowego do zbadania pełnej aplikacji, funkcjonującej zarówno w środowisku domyślnym, łącząc się z serwerem, jak i odtwarzając ją na w odizolowanym środowisku testowym. Aplikacja testowana będzie zarówno na systemie Windows 11, jak i Ubuntu 22.04.

## 7. Kryteria sukcesu/porażku

Test uznaje się za zaliczony, jeśli:
- badane funkcjonalności zachowują się w sposób opisany w specyfikacji wymagań
- nie występują krytyczne błędy w działaniu systemu
- elementy systemu działają zgodnie z oczekiwaniami i ustalonymi standardami systemów POS
- podczas testów wydajności w przypadkach skrajnych system działa w podobnie niezawodny sposób, co w normalnych warunkach

Test uznaje się za niezaliczony, jeśli:
- którekolwiek z wymaganych funkcjonalności nie są spełnione
- występują błędy krytyczne
- system nie daje odpowiedniej informacji zwrotnej w przynajmniej jednym przypadku testowym
- system zachowuje się w sposób nieoczekiwany

## 8. Kryteria wstrzymania testów oraz wymagania ich wznowienia

Proces testowania zostanie wstrzymany w przypadku wykrycia problemów z uruchomieniem aplikacji w danych warunkach bądź wykrycia defektów uszkadzających go w sposób trwały. Zostanie on wznowiony po naprawieniu problemów i przywróceniu pełnej dostępności środowiska.

## 9. Efekty końcowe testów

Po wykonaniu testów dostarczona zostanie dokumentacja wykonanych przypadków testowych oraz raport końcowy.

## 10. Zadania w ramach testów

- przygotowanie przypadków testowych pokrywających wszystkie wymagania zawartym w specyfikacji
- staranne wykonanie testów w taki sposób, aby każde wymaganie zostało zweryfikowane w różnych scenariuszach i warunkach
- przygotowanie dokumentacji wykonanych testów oraz sporządzenie raportu końcowego

## 11. Wymagania środowiskowe

Komputery z systemami Windows 11 oraz Ubuntu 22.04, a także dostęp do internetu.

## 12. Odpowiedzialność

Odpowiedzialnym za zaprojektowanie, przygotowanie, wykonanie i udokumentowanie testów jest Krzysztof Czarnowus, jedyny członek grupy Kryzys.

## 13. Harmonogram

Dokładny harmonogram wykonanych testów zależy od wymagań przedstawionych przez prowadzącego na ćwiczeniach. Kolejne etapy odbędą się jednak w następującej kolejności:
1. Przygotowanie przypadków testowych.
2. Krytyczna analiza pokrycia wymagań zawartych w specyfikacji.
3. Przeprowadzenie testów powiązanych z wymaganiami funkcjonalnymi na systemie zainstalowanym na odizolowanym urządzeniu.
4. Przeprowadzenie testów powiązanych z wymaganiami niefunkcjonalnymi na systemie zainstalowanym na odizolowanym urządzeniu.
5. Przygotowanie dokumentacji wykonanych testów oraz analiza, które testy należy powtórzyć na systemie funkcjonującym na zewnętrznym serwerze.
6. Przeprowadzenie wybranych testów na systemie funkcjonującym na zewnętrznym serwerze.
7. Przygotowanie dokumentacji wykonanych testów.
8. Analiza wyników oraz przygotowanie ostatecznego raportu z testów.

## 14. Ryzyka i nieprzewidziane zdarzenia

- ryzyko: problemy z uruchomieniem systemu na własnym urządzeniu
- rozwiązania: skontaktowanie się z twórcą, konsultacje z bardziej doświadczonymi programistami, ograniczenie testów do tych wykonywanych na systemie funkcjonującym na zewnętrznym serwerze

- ryzyko: problemy z odpowiednim przygotowaniem dokumentacji wynikające z braku znajomości standardów
- rozwiązania: konsultacja z prowadzącym dotycząca formy opisywania wykonywania przypadków testowych

## 15. Zatwierdzanie

Plan testów musi zostać zatwierdzony przez prowadzącego ćwiczenia.

## 16. Repozytorium

Repozytorium projektu znajduje się pod linkiem:
[LINK DO REPOZYTORIUM](https://github.com/maksiu106/TestowanieOprogramowania)
