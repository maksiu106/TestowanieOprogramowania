# Ogólne przypadki testowe dla systemu ewidencji herbaciarni Czajownia

### TC-TEASHOP-01

- opis: weryfikacja procesu tworzenia zamówienia
- cel: sprawdzenie, czy tworzenie zamówienia umożliwia niezawodne wprowadzenie wszystkich potrzebnych danych
- wymagania: REQ-FUNC-001, REQ-NFUNC-005

### TC-TEASHOP-02

- opis: weryfikacja modyfikacji parametrów zamówienia
- cel: sprawdzenie, czy można modyfikować otwarte zamówienia
- wymagania: REQ-FUNC-001, REQ-NFUNC-005

### TC-TEASHOP-03

- opis: weryfikacja przypisywania zamówień miejscu na sali oraz poprawnego sortowania
- cel: sprawdzenie, czy zachowanie systemu po przypisaniu zamówieniu stolika jest zgodne z oczekiwaniami pracownika
- wymagania: REQ-FUNC-002, REQ-NFUNC-005

### TC-TEASHOP-04 

- opis: weryfikacja funkcjonalności związanych z listą dostępnych towarów
- cel: sprawdzenie, czy archiwum dostępnych towarów funkcjonuje zgodnie z oczekiwaniami
- wymagania: REQ-FUNC-003, REQ-NFUNC-001

### TC-TEASHOP-05

- opis: weryfikacja funkcjonalności związanych z rezerwacjami
- cel: sprawdzenie funkcjonalności wprowadzania, modyfikacji i usuwania rezerwacji
- wymagania: REQ-FUNC-004, REQ-NFUNC-001, REQ-NFUNC-002

### TC-TEASHOP-06

- opis: weryfikacja przejrzystego sortowania przyjętych rezerwacji
- cel: sprawdzenie, czy w procesie dodawania i modyfikowania rezerwacji system w odpowiedni sposób je układa
- wymagania: REQ-FUNC-004, REQ-NFUNC-001

### TC-TEASHOP-07

- opis: weryfikacja działania systemu przy wprowadzaniu niepoprawnych danych
- cel: sprawdzenie, czy system jest zabezpieczony na wypadek wprowadzania niepoprawnych parametrów w funkcjach zarządzania zamówieniami, rezerwacjach bądź archiwum
- wymagania: REQ-FUNC-001, REQ-FUNC-002, REQ-FUNC-003, REQ-FUNC-004, REQ-NFUNC-001

### TC-TEASHOP-08

- opis: weryfikacja archiwum zamówień
- cel: sprawdzenie, czy podczas zamykania zamówień wszystkie w odpowiedni sposób trafiają do archiwum i są sumowane zgodnie z oczekiwaniami
- wymagania: REQ-FUNC-005, REQ-NFUNC-005

### TC-TEASHOP-09

- opis: weryfikacja możliwości obsługiwania systemu na wielu urządzeniach synchronicznie
- cel: sprawdzenie, czy możliwe jest połączenie się z systemem na dwóch różnych urządzeniach/platformach, a także czy wprowadzane dane są odpowiednio odświeżane na obu
- wymagania: REQ-FUNC-006, REQ-NFUNC-001

### TC-TEASHOP-10

- opis: weryfikacja możliwości uruchomienia programu na lokalnym urządzeniu
- cel: sprawdzenie, czy system uruchomiony na lokalnym urządzeniu działa identycznie z systemem uruchomionym na zewnętrznym serwerze
- wymagania: REQ-FUNC-007

### TC-TEASHOP-11

- opis: weryfikacja odpowiedzi zwrotnych systemu przy wykonywaniu działań
- cel: sprawdzenie przejrzystości komunikacji systemu z pracownikiem i informacji o powodzeniu bądź niepowodzeniu podjętych działań 
- wymagania: REQ-FUNC-008, REQ-NFUNC-001, REQ-NFUNC-005

### TC-TEASHOP-12

- opis: weryfikacja przeciwdziałania systemu niepożądanemu dublowaniu podjętych akcji
- cel: sprawdzenie, czy system jest zabezpieczony przed nadpobudliwością pracowników wykonujących kilkukrotnie jedno działanie
- wymagania: REQ-FUNC-009, REQ-NFUNC-001, REQ-NFUNC-005

### TC-TEASHOP-13

- opis: weryfikacja czasu odpowiedzi programu podczas wykonywania podstawowych funkcji
- cel: sprawdzenie, czy system działa odpowiednio szybko oraz czy w przypadku wydłużonego czasu procesowania poleceń podaje odpowiednią wiadomość zwrotną
- wymagania: REQ-NFUNC-001

### TC-TEASHOP-14

- opis: weryfikacja niezawodności systemu w aspekcie przechowywania rezerwacji
- cel: sprawdzenie, czy wprowadzone informacje o rezerwacjach są przechowywane w systemie przez odpowiednio długi czas
- wymagania: REQ-NFUNC-002

### TC-TEASHOP-15

- opis: weryfikacja bezpieczeństwa systemu związanego z autoryzacją pracowników
- cel: sprawdzenie, czy spełnione są podstawowe wymagania uniemożliwiające wejście do systemu i modyfikowaniu zawartości bazy danych osobom z zewnątrz
- wymagania: REQ-NFUNC-003

### TC-TEASHOP-16

- opis: weryfikacja przejrzystości i przyswajalności systemu nowym pracownikom
- cel: sprawdzenie, czy nowo zatrudniony pracownik jest w stanie łatwo przyswoić funkcjonowanie systemu i wykonanie podstawowych akcji po 10-minutowym szkoleniu
- wymagania: REQ-NFUNC-004

### TC-TEASHOP-17

- opis: weryfikacja podobieństwa systemu do innych programów służących obsłudze zamówień w gastronomii
- cel: sprawdzenie, czy system jest zgodny z ogólnie przyjętymi standardami programów POS
- wymagania: REQ-NFUNC-004

### TC-TEASHOP-18

- opis: weryfikacja czasu odpowiedzi podczas wykonywania kluczowych funkcji wykorzystywanych z dużą częstotliwością
- cel: sprawdzenie, czy natychmiastowe wprowadzanie dużych ilości danych nie prowadzi do nieprzewidzanych zachowań systemu
- wymagania: REQ-NFUNC-005

### TC-TEASHOP-19

- opis: porównanie wydajności działania systemu uruchamianego na lokalnym urządzeniu oraz podczas łączenia się z nim przez serwer
- cel: sprawdzenie, czy najważniejsze testy wykonane w izolowanym środowisku testowym dają identyczną odpowiedź, co w działającym środowisku docelowym
- wymagania: REQ-FUNC-005, REQ-FUNC-006, REQ-FUNC-008, REQ-FUNC-009, REQ-NFUNC-001, REQ-NFUNC-002, REQ-NFUNC-003, REQ-NFUNC-005, REQ-NFUNC-006

