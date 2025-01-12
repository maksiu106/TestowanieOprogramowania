# Niskopoziomowe przypadki testowe dla systemu ewidencji herbaciarni Czajownia

### TC-TEASHOP-01-01

- **cel**: sprawdzenie, czy tworzenie zamówienia umożliwia niezawodne wprowadzenie wszystkich potrzebnych danych
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego
- **kroki**:
	1. Kliknij "Nowe zamówienie".
	2. Ustaw wszystkie potrzebne parametry zamówienia, takie jak: towar, rodzaj sprzedaży, cenę, zniżkę oraz stolik - wprowadź w odpowiednio podpisane okienka.
	3. Dodaj kolejny towar do utworzonego zamówienia.
	4. Zaznacz, że zamówienie zostało już opłacone, a później również wyniesione i zamknięte.
- **oczekiwane wyniki**: system umożliwił utworzenie zamówienia, wprowadzenie jego parametrów oraz poprawnie zareagował na jego zamknięcie.

### TC-TEASHOP-02-01

- **cel**: sprawdzenie, czy można modyfikować otwarte zamówienia
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, istnieje już utworzone zamówienie z kilkoma towarami
- **kroki**:
	1. Usuń jeden z towarów w zamówieniu.
	2. Zmień drugi z towarów w zamówieniu na jakiś inny.
	3. Zmień rodzaj sprzedaży zmienionego towaru.
	4. Zmień zaznaczony stolik zamówienia.
- **oczekiwane wyniki**: system umożliwił zmodyfikowanie odpowiednich parametrów zamówienia.

### TC-TEASHOP-03-01

- **cel**: sprawdzenie, czy zachowanie systemu po przypisaniu zamówieniu stolika odpowiada wymaganiom - to znaczy, czy są one sortowane w odpowiedniej kolejności.
- **wyjaśnienie**: stoliki oznaczone są literami sal (kolejno: b, s, o, m) oraz numerem stolika. Przykładowe oznaczenie: b3.
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, istnieje utworzonych kilka zamówień bez przypisanych stolików.
- **kroki**:
	1. Wprowadź nazwy kilku stolików zgodnie z przyjętą konwencją.
	2. Przypisz po jednym stoliku w każdej sali.
	3. W jednej z sal wprowadź więcej niż jeden stolik.
- **oczekiwane wyniki**: zamówienia są sortowane w zależności od oznaczenia sali i numeru stolika.

### TC-TEASHOP-04-01

- **cel**: sprawdzenie, czy archiwum dostępnych towarów funkcjonuje zgodnie z oczekiwaniami - czy szukanie towaru nie jest uciążliwe, a także czy możliwa jest modyfikacja listy.
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, istnieje otwarte zamówienie z wprowadzonym jednym towarem
- **kroki**:
	1. Ręcznie zmień cenę wprowadzanego towaru w otwartym zamówieniu.
	2. W pasku górnym kliknij "Magazyn".
	3. Zmodyfikuj cenę wybranego towaru.
	4. Wprowadź nowy towar, ustaw jego nazwę i cenę.
	5. Wróć do ekranu głównego i dodaj do otwartego zamówienia utworzony wcześniej towar.
- **oczekiwane wyniki**: system umożliwił dodanie nowego towaru oraz dynamiczną zmianę ceny w otwartym zamówieniu.

### TC-TEASHOP-05-01

- **cel**: sprawdzenie funkcjonalności wprowadzania, modyfikacji i usuwania rezerwacji
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego
- **kroki**:
	1. W pasku górnym kliknij "Rezerwacje".
	2. Utwórz nową rezerwację.
	3. Wprowadź odpowiednie parametry - imię, godzinę i datę oraz stolik.
	4. Zapisz rezerwację.
	5. Edytuj utworzoną wcześniej rezerwację, zmieć któreś z parametrów i zapisz ponownie.
	6. Usuń stworzoną rezerwację.
- **oczekiwane wyniki**: system poprawnie zapisywał każdą modyfikację i wyświetlał poprawne zmieniane dane.

### TC-TEASHOP-06-01

- **cel**: sprawdzenie, czy w procesie dodawania i modyfikowania rezerwacji system w odpowiedni sposób je sortuje i układa na ekranie
- **warunki wstępne**: autoryzowany użytkownik ma dostęp do ekranu głównego
- **kroki**:
	1. W pasku górnym kliknij "Rezerwacje".
	2. Utwórz dwie rezerwacje w różnym czasie.
	3. Sprawdź, czy zostały one posortowane chronologicznie.
	4. Zmodyfikuj późniejszą rezerwację, aby była ona wcześniej od tej drugiej.
	5. Zapisz modyfikację.
	6. Sprawdź, czy system ponownie uporządkował rezerwacje.
	
- **oczekiwane wyniki**: Rezerwacje zamieniły się miejscami i są poprawnie posortowane chronologicznie.

### TC-TEASHOP-07-01

- **cel**: sprawdzenie zachowania systemu po wprowadzeniu niepoprawnej nazwy stolika w zamówieniu
- **wyjaśnienie**: stoliki oznaczone są literami sal (kolejno: b, s, o, m) oraz numerem stolika. Przykładowe oznaczenie: b3.
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, istnieje utworzonych kilka zamówień bez przypisanych stolików.
- **kroki**:
	1. Utwórz kilka zamówień.
	1. Wprowadź nazwy kilku stolików zgodnie z przyjętą konwencją.
	2. Wprowadź niepoprawną nazwę stolika.
- **oczekiwane wyniki**: system rozpoznaje nieprawidłową nazwę stolika i nie sortuje zamówienia.

### TC-TEASHOP-07-02

- **cel**: sprawdzenie, czy archiwum towarów ma wprowadzone zabezpieczenia na wypadek wprowadzania niewłaściwych wartości i przepełniania bufora znaków.
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego
- **kroki**:
	1. W pasku górnym kliknij "Magazyn".
	2. Wprowadź nowy towar.
	3. Jako nazwę towaru wprowadź możliwie najdłuższy ciąg znaków.
	4. Jako cenę towaru wprowadź ciąg tekstowy.
	5. Wróć do ekranu głównego.
	6. Utwórz nowe zamówienie, używając stworzonego towaru.
- **oczekiwane wyniki**: ilość ponadlimitowych znaków w nazwie towaru zostanie ucięta, a niewłaściwa wartość ceny albo nie zostanie zaakceptowana przez system, albo nie będzie się wliczała do podsumowania ceny zamówienia.

### TC-TEASHOP-07-03

- **cel**: sprawdzenie zabezpieczeń systemu rezerwacji przed wprowadzaniem niewłaściwych parametrów i przepełnienia bufora znaków
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego
- **kroki**:
	1. W pasku górnym kliknij "Rezerwacje".
	2. Utwórz nową rezerwację.
	3. W którymś z pól wprowadź możliwie jak najdłuższy ciąg znaków.
	4. Zapisz rezerwację.
- **oczekiwane wyniki**: ilość ponadlimitowych znaków w odpowiednim oknie zostanie ograniczona do dozwolonego limitu.

### TC-TEASHOP-08-01

- **cel**: sprawdzenie, czy podczas zamykania zamówień wszystkie w odpowiedni sposób trafiają do archiwum i są sumowane zgodnie z oczekiwaniami
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego
- **kroki**:
	1. Utwórz kilka zamówień, każde z kilkoma towarami.
	2. Zamknij zamówienia.
	3. W pasku górnym wybierz "Archiwum".
	4. Sprawdź, czy zamknięte zamówienia znalazły się w archiwum, a także czy podsumowanie ceny zgadza się z wartością faktyczną.
	5. Kliknij przycisk "Przywróć"
	6. Wróć do ekranu głównego i sprawdź, czy przywrócone zamówienie znajduje się na liście, wraz ze wszystkimi wprowadzonymi wcześniej parametrami.
- **oczekiwane wyniki**: system sprawnie przenosi wszystkie zamówienia do archiwum po ich zamknięciu i odpowiednio sumuje utarg dobowy, również po przywróceniu zamówienia.

### TC-TEASHOP-09-01

- **cel**: sprawdzenie, czy możliwe jest połączenie się z systemem na dwóch różnych urządzeniach/platformach, a także czy wprowadzane dane są odpowiednio odświeżane na obu
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego na dwóch różnych platformach/urządzeniach (w przypadku pracy na systemie uruchomionym w środowisku testowym - na dwóch różnych przeglądarkach)
- **kroki**:
	1. Utwórz zamówienie z dowolnymi parametrami na jednym urządzeniu.
	2. Na drugim urządzeniu utwórz inne zamówienie w ramach systemu połączonym z tym samym serwerem.
	3. Porównaj, czy zamówienia wprowadzane na jednym urządzeniu pojawiają się również na drugim.
- **oczekiwane wyniki**: Zmiany wprowadzane na jednej platformie/urządzeniu stają się w krótkim czasie widoczne na drugim.

### TC-TEASHOP-10-01

- **cel**: sprawdzenie, czy system uruchomiony na lokalnym urządzeniu działa identycznie z systemem uruchomionym na zewnętrznym serwerze
- **warunki wstępne**: dostęp do systemu uruchomionego w środowisku docelowym, system postawiony na lokalnym serwerze, zautoryzowany użytkownik ma dostęp do ekranu głównego
- **kroki**:
	1. Wybierz najważniejsze z testów wykonanych w odizolowanym środowisku testowym.
	2. Powtórz przypadki testowe w środowisku docelowym.
- **oczekiwane wyniki**: Zachodzi pełna zgodność w zachowaniu systemu w obu przypadkach.

### TC-TEASHOP-11-01

- **cel**: sprawdzenie przejrzystości komunikacji systemu z pracownikiem i informacji o powodzeniu bądź niepowodzeniu podjętych działań
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego
- **kroki**:
	1. Wybierz wśród wykonanych testów te, w których czas oczekiwania na odpowiedź systemu był zauważalnie większy.
	2. Powtórz przypadki testowe.
	3. Zwracaj uwagę na obecność bądź nieobecność informacji zwrotnych.
- **oczekiwane wyniki**: System podaje informację zwrotną dla wszystkich akcji, które zajmują zauważalnie większą ilość czasu.

### TC-TEASHOP-12-01

- **cel**: sprawdzenie zachowania systemu przy natychmiastowym wprowadzeniu kilku różnych parametrów zamówienia
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, tester posiada zainstalowany wybrany program do automatyzacji kliknięć (np. Actiona na systemie Ubuntu)
- **kroki**:
	1. Kliknij "Nowe zamówienie".
	2. Wprowadź dwa dowolne towary.
	3. Za pomocą systemu do automatyzacji kliknięć zaznacz status wyniesienia obu towarów oraz status opłacenia zamówienia - każdy w odstępie 0.5 s.
- **oczekiwane wyniki**: system poprawnie zaznaczył wszystkie wprowadzone dane.

### TC-TEASHOP-12-02

- **cel**: sprawdzenie, czy archiwum towarów ma zabezpieczenia na wypadek zbyt długiego czasu procesowania
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, tester posiada zainstalowany wybrany program do automatyzacji kliknięć (np. Actiona na systemie Ubuntu)
- **kroki**:
	1. W pasku górnym kliknij "Magazyn".
	2. Wprowadź dowolny nowy towar do bazy danych.
	3. Za pomocą narzędzia do automatyzacji kliknięć kliknij kilkukrotnie w odstępie czasu 0.5 s zapisanie wprowadzonego rodzaju towaru.
- **oczekiwane wyniki**: system wprowadzi do bazy tylko jeden nowy towar, opcjonalnie wyświetlając komunikat.

### TC-TEASHOP-12-03

- **cel**: sprawdzenie zachowania systemu przy kilkukrotnym kliknięciu zapisania rezerwacji
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, tester posiada zainstalowany wybrany program do automatyzacji kliknięć (np. Actiona na systemie Ubuntu)
- **kroki**:
	1. W pasku górnym kliknij "Rezerwacje".
	2. Utwórz nową rezerwację.
	3. Wprowadź odpowiednie parametry - imię, godzinę i datę oraz stolik.
	4. Za pomocą programu do automatyzacji kliknięć wykonaj kilkukrotne zapisanie rezerwacji w odstępie 0.5 s.
- **oczekiwane wyniki**: system zapisał rezerwację tylko jednokrotnie, ewentualnie wyświetlając odpowiedni komunikat.

### TC-TEASHOP-12-04

- **cel**: sprawdzenie, czy system posiada zabezpieczenia na wypadek kilkukrotnego wysłania zamówienia do archwium bądź przywrócenia go.
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, tester posiada zainstalowany wybrany program do automatyzacji kliknięć (np. Actiona na systemie Ubuntu) 
- **kroki**:
	1. Stwórz zamówienie i wprowadź jego dowolne parametry.
	2. Za pomocą programu do automatyzacji kliknięć zamknij zamówienie kilkukrotnie w odstępie 0.5 s.
	3. W pasku górnym wybierz "Archiwum".
	4. Rozwiń zamknięte zamówienie i za pomocą programu do automatyzacji kliknięć przywróć zamówienie kilkukrotnie w odstępie 0.5 s.
- **oczekiwane wyniki**: kilkurkotne kliknięcie przycisku nie wpływa na powielenie zamówień - ani podczas przesyłania go do archiwum, ani podczas przywracania.

### TC-TEASHOP-14-01

- **cel**: sprawdzenie czasu przechowywania rezerwacji przez system
- **warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego i dwa tygodnie czasu
- **kroki**:
	1. Utwórz rezerwację z terminem dwóch tygodni od momentu jej wprowadzenia.
	2. Dzień przed wprowadzoną datą sprawdź, czy rezerwacja wciąż jest przechowywana przez system.
- **oczekiwane wyniki**: Rezerwacja wciąż znajduje się na liście.

### TC-TEASHOP-15-01

- **cel**: weryfikacja bezpieczeństwa systemu związanego z autoryzacją pracowników
- **warunki wstępne**: niezweryfikowany użytkownik ma dostęp do strony głównej
- **kroki**:
	1. Spróbuj wykonać jakiekolwiek działanie w systemie.
- **oczekiwane wyniki**: Użytkownik bez autoryzacji nie jest w stanie zajrzeć do systemu, wykonać żadnego działania ani sprawdzić żadnych danych.

### TC-TEASHOP-16-01

- **cel**: sprawdzenie, czy nowo zatrudniony pracownik jest w stanie łatwo przyswoić funkcjonowanie systemu i wykonanie podstawowych akcji
- **warunki wstępne**: dostęp do osoby, która nie miała styczności z testowanym systemem, umożliwienie jej dostępu do ekranu głównego
- **kroki**:
	1. Polecić osobie stworzyć zamówienie oraz wprowadzić jego zadane dowolne parametry, nie podając szczegółów, jak to zrobić.
	2. Polecić osobie stworzyć rezerwację.
- **oczekiwane wyniki**: Użytkownik nieznający systemu po chwili szukania odpowiednich elementów na stronie jest w stanie wykonać najprostsze akcje.

### TC-TEASHOP-17-01

- **cel**: sprawdzenie, czy system jest zgodny z ogólnie przyjętymi standardami programów POS
- **warunki wstępne**: dostęp do internetu, zautoryzowany użytkownik ma dostęp do ekranu głównego
- **kroki**:
	1. Znajdź w internecie sensownie wyglądającą listę wymagań dotyczących systemów POS.
	2. Sprawdź, czy testowane oprogramowanie spełnia dane wymagania.
- **oczekiwane wyniki**: Testowany system jest systemem dedykowanym, więc nie musi spełniać wszystkich ogólnie przyjętych standardów. Spodziewane są pewne rozbieżności, wynikające ze specyfiki systemu i dostosowania go do konkretnych warunków.
