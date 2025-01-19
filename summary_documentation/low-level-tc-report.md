# Raport wykonania niskopoziomowych przypadków testowych systemu ewidencji herbaciarni Czajownia

**data wykonania**: 19.01.2024
**osobowa odpowiedzialna za przygotowanie raportu**: Krzysztof Czarnowus
**cel**: podsumowanie wykonania niskopoziomowych przypadków testowych

## TC-TEASHOP-01-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-01-01
- **opis**: sprawdzenie, czy tworzenie zamówienia umożliwia niezawodne wprowadzenie wszystkich potrzebnych danych
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Kliknij "Nowe zamówienie". | Kliknięto odpowiedni przycisk. | zaliczony |
| 2 | Ustaw wszystkie potrzebne parametry zamówienia, takie jak: towar, rodzaj sprzedaży, cenę, zniżkę oraz stolik - wprowadź w odpowiednio podpisane okienka. | Wybrano pierwszy dostępny towar z rozwijanej listy, wprowadzono zniżkę 5% na zamówienie oraz przypisano stolik "o2". | zaliczony |
| 3 | Dodaj kolejny towar do utworzonego zamówienia. | Z rozwijanej listy wybrano drugi dostępny towar. | zaliczony |
| 4 | Zaznacz, że zamówienie zostało już opłacone, a później również wyniesione i zamknięte. | Zaznaczono odpowiednie przyciski. | zaliczony |

**uwagi**: brak

## TC-TEASHOP-02-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-02-01
- **opis**: sprawdzenie, czy można modyfikować otwarte zamówienia
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, istnieje już utworzone zamówienie z kilkoma towarami

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Usuń jeden z towarów w zamówieniu. | Usunięto drugi z towarów w otwartym w poprzednim przypadku testowym zamówieniu. | zaliczony |
| 2 | Zmień drugi z towarów w zamówieniu na jakiś inny. | Wymieniono pierwszy towar na inny z rozwijanej listy. | zaliczony |
| 3 | Zmień rodzaj sprzedaży zmienionego towaru. | Zamieniono typ towaru z domyślnego "sztuka" na "gram" | zaliczony |
| 4 | Zmień zaznaczony stolik zamówienia. | Zmieniono stolik na "b3". | zaliczony |

**uwagi**: brak

## TC-TEASHOP-03-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-03-01
- **opis**: sprawdzenie, czy zachowanie systemu po przypisaniu zamówieniu stolika odpowiada wymaganiom - to znaczy, czy są one sortowane w odpowiedniej kolejności.
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, istnieje utworzonych kilka zamówień bez przypisanych stolików.

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Wprowadź nazwy kilku stolików zgodnie z przyjętą konwencją. | Wprowadzono do dwóch różnych stolików nazwy "m4" oraz "b7". | zaliczony |
| 2 | Przypisz po jednym stoliku w każdej sali. | Dodano również dwa nowe zamówienia i ustawiono ich nazwy jako "o9" oraz "s5". | zaliczony |
| 3 | W jednej z sal wprowadź więcej niż jeden stolik. | Dodano nowe zamówienie i przypisano mu stolik "o1" | zaliczony |

**uwagi**: brak

## TC-TEASHOP-04-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-04-01
- **opis**: sprawdzenie, czy archiwum dostępnych towarów funkcjonuje zgodnie z oczekiwaniami - czy szukanie towaru nie jest uciążliwe, a także czy możliwa jest modyfikacja listy.
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, istnieje otwarte zamówienie z wprowadzonym jednym towarem.

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Ręcznie zmień cenę wprowadzanego towaru w otwartym zamówieniu. | Zmieniono cenę wybranego towaru na 30 zł. | zaliczony |
| 2 | W pasku górnym kliknij "Magazyn". | Wybrano odpowiedni przycisk, przechodząc do listy towarów. | zaliczony |
| 3 | Zmodyfikuj cenę wybranego towaru. | Zmieniono nazwę towaru "akcesoria" w wersji "opakowanie" na 10 zł. | zaliczony |
| 4 | Wprowadź nowy towar, ustaw jego nazwę i cenę. | Wybrano opcję tworzenia nowego produktu, nazwano go "test" oraz wprowadzono cenę 2000 zł. | zaliczony |
| 5 | Wróć do ekranu głównego i dodaj do otwartego zamówienia utworzony wcześniej towar. | Dodano odpowiedni towar do zamówienia. | zaliczony |

**uwagi**: brak

## TC-TEASHOP-05-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-05-01
- **opis**: sprawdzenie funkcjonalności wprowadzania, modyfikacji i usuwania rezerwacji
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego.

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | W pasku górnym kliknij "Rezerwacje". | Wybrano odpowiedni przycisk. | zaliczony |
| 2 | Utwórz nową rezerwację. | Wybrano odpowiedni przycisk. | zaliczony |
| 3 | Wprowadź odpowiednie parametry - imię, godzinę i datę oraz stolik. | Wprowadzono imię, stolik, godzinę i datę - tą ostatnią na 2055 rok. | zaliczony |
| 4 | Zapisz rezerwację. | Zapisano rezerwację, która wyświetliła się na liście na samym końcu, odpowiednio posortowana chronologicznie. | zaliczony |
| 5 | Edytuj utworzoną wcześniej rezerwację, zmieć któreś z parametrów i zapisz ponownie. | Wybrano przycisk edycji rezerwacji i zmieniono datę na aktualny dzień z godzinnym wyprzedzeniem. Po zapisaniu stwierdzono ponowne poprawne posortowanie chronologiczne obecnych rezerwacji. | zaliczony |
| 6 | Usuń stworzoną rezerwację. | Wybrano przycisk edycji rezerwacji i usunięto ją. | zaliczony |

**uwagi**: brak

## TC-TEASHOP-06-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-06-01
- **opis**: sprawdzenie, czy w procesie dodawania i modyfikowania rezerwacji system w odpowiedni sposób je sortuje i układa na ekranie
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego.

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | W pasku górnym kliknij "Rezerwacje". | Wybrano odpowiedni przycisk. | zaliczony |
| 2 | Utwórz dwie rezerwacje w różnym czasie. | Stworzono dwie rezerwacje w dwa różne dni - najpierw późniejszą, potem wcześniejszą. | zaliczony |
| 3 | Sprawdź, czy zostały one posortowane chronologicznie. | Zaobserwowano poprawne sortowanie. | zaliczony |
| 4 | Zmodyfikuj późniejszą rezerwację, aby była ona wcześniej od tej drugiej. | Wybrano przycisk edycji późniejszej rezerwacji i zmieniono odpowiedni datę i godzinę. | zaliczony |
| 5 | Zapisz modyfikację. | Zapisano wykonaną modyfikację. | zaliczony |
| 6 | Sprawdź, czy system ponownie uporządkował rezerwacje. | Zaobserwowano ponowne poprawne posortowanie chronologiczne. | zaliczony |

**uwagi**: brak

## TC-TEASHOP-07-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-07-01
- **opis**: sprawdzenie zachowania systemu po wprowadzeniu niepoprawnej nazwy stolika w zamówieniu
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: orange;">częściowo zaliczony</span>

### Opis wykonania

**warunki wstępne**: autoryzowany użytkownik ma dostęp do ekranu głównego, istnieje utworzonych kilka zamówień bez przypisanych stolików.

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Utwórz kilka zamówień. | Utworzono trzy zamówienia. | zaliczony |
| 2 | Wprowadź nazwy kilku stolików zgodnie z przyjętą konwencją. | Dla dwóch z utworzonych zamówień wprowadzono nazwy "b304" oraz "m70". Zaobserwowano poprawne posortowanie zamówień oraz podświetlenie ich zgodnie z kolorem sali. | zaliczony |
| 3 | Wprowadź niepoprawną nazwę stolika. | Wprowadzono nazwę stolika, która jest przekopiowaną treścią "Pana Tadeusza". Cała treść została wprowadzona, po czym zaobserwowano gwałtowny spadek czasu odpowiedzi systemu. Stolik z nieprawidłową nazwą nie został posortowany ani podświetlony. | <span style="color: orange;">częściowo zaliczony</span> |

**uwagi**: System poprawnie rozpoznaje dopuszczalne nazwy stolików i odpowiedni jest sortuje, zauważono jednak, że pole nazwy stolika nie ma dopuszczalnego bufora znaków, pozwalając na wprowadzenie nielimitowanej ich ilości, co może w ekstremalnych przypadkach przełożyć się na gwałtowne pogorszenie wydajności funkcjonowania systemu.

## TC-TEASHOP-07-02

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-07-02
- **opis**: sprawdzenie, czy archiwum towarów ma wprowadzone zabezpieczenia na wypadek wprowadzania niewłaściwych wartości i przepełniania bufora znaków.
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | W pasku górnym kliknij "Magazyn". | Wybrano odpowiednią zakładkę. | zaliczony |
| 2 | Wprowadź nowy towar. | Wybrano opcję tworzenia nowego produktu. | zaliczony |
| 3 | Jako nazwę towaru wprowadź długi ciąg znaków | W odpowiednie pole przekopiowano wiersz Morsztyna "Do Kanikuły". Cała treść została dopuszczona. | <span style="color: red;">niezaliczony</span> |
| 4 | Jako cenę towaru wprowadź ciąg tekstowy. | Spróbowano wprowadzić ciąg liter, na co system nie pozwolił. | zaliczony |
| 5 | Wróć do ekranu głównego. | Powrócono do ekranu głównego. | zaliczony |
| 6 | Utwórz nowe zamówienie, używając stworzonego towaru. | Utworzono zamówienie, wybierając towar, którego nazwa jest barokowym wierszem. Zauważono wyraźny spadek czasu odpowiedzi systemu. | zaliczony |

**uwagi**: System nie posiada zabezpieczeń na wypadek przepełnienia pola nazwy towaru i zezwala na utworzenie nieograniczenie długiego ciągu znaków, co przekłada się na zauważalny spadek jego wydajności i wprowadza ryzyko awarii.

## TC-TEASHOP-07-03

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-07-03
- **opis**: sprawdzenie zabezpieczeń systemu rezerwacji przed wprowadzaniem niewłaściwych parametrów i przepełnienia bufora znaków
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | W pasku górnym kliknij "Rezerwacje". | Wybrano odpowiednią zakładkę. | zaliczony |
| 2 | Utwórz nową rezerwację. | Wybrano przycisk tworzenia rezerwacji. Zaobserwowano wyłączenie systemu i pokazywanie pustej strony. Po odczekaniu około minuty ponowiono próbę, obserwując poprawne wyświetlenie okienka dodawania rezerwacji. | <span style="color: red;">niezaliczony</span> |
| 3 | W którymś z pól wprowadź możliwie jak najdłuższy ciąg znaków. | W pole do uwag dotyczących zamówienia wprowadzono całą treść "Przedwiośnia" Stefana Żeromskiego, na co system pozwolił. Zaobserwowano gwałtowny spadek czasu odpowiedzi systemu. | <span style="color: red;">niezaliczony</span> |
| 4 | Zapisz rezerwację. | Ze względu na ryzyko awarii, nie zdecydowano się na zapisanie rezerwacji z błędnymi danymi | brak |

**uwagi**: System nie posiada zabezpieczeń na wypadek przepełnienia pól tekstowych przy tworzeniu rezerwacji i zezwala na utworzenie nieograniczenie długiego ciągu znaków, co przekłada się na zauważalny spadek jego wydajności i wprowadza ryzyko awarii.

## TC-TEASHOP-08-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-08-01
- **opis**: sprawdzenie, czy podczas zamykania zamówień wszystkie w odpowiedni sposób trafiają do archiwum i są sumowane zgodnie z oczekiwaniami
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Utwórz kilka zamówień, każde z kilkoma towarami. | Utworzono dwa różne zamówienia, z różnymi towarami, zaznaczając stolik, wyniesienie oraz odznaczając, że zostały opłacone. | zaliczony |
| 2 | Zamknij zamówienia. | Zamknięto oba. | zaliczony |
| 3 | W pasku górnym wybierz "Archiwum". | Wybrano odpowiednią zakładkę. | zaliczony |
| 4 | Sprawdź, czy zamknięte zamówienia znalazły się w archiwum, a także czy podsumowanie ceny zgadza się z wartością faktyczną. | Potwierdzono obecność obu zamówień i poprawne zsumowanie ich kwoty. | zaliczony |
| 5 | Kliknij przycisk "Przywróć" | Wybrano odpowiedni przycik. | zaliczony |
| 6 | Wróć do ekranu głównego i sprawdź, czy przywrócone zamówienie znajduje się na liście, wraz ze wszystkimi wprowadzonymi wcześniej parametrami. | Przywrócono oba zamówienia, które pojawiły się na ekranie głównym. Zniknęła jednak informacja o ich statusie opłacenia oraz stopniu przygotowania - jedynie stolik pozostał zaznaczony. | <span style="color: red;">niezaliczony</span> |

**uwagi**: Zaobserwowano, że przy przywracaniu zamówień z archiwum giną wszystkie informacje o nich poza listą zamówionych w ich ramach towarów. Może to być celowa architektura, mająca na celu zmniejszenie ilości przechowywanych informacji, jednak prawdopodobnie w niektórych przypadkach może wyraźnie brakować tej funkcjonalności.

## TC-TEASHOP-09-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-09-01
- **opis**: sprawdzenie, czy możliwe jest połączenie się z systemem na dwóch różnych urządzeniach/platformach, a także czy wprowadzane dane są odpowiednio odświeżane na obu
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego na dwóch różnych przeglądarkach internetowych

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Utwórz zamówienie z dowolnymi parametrami na jednym urządzeniu. | Utworzono odpowiednie zamówienie i wprowadzono kilka towarów. | zaliczony |
| 2 | Na drugim urządzeniu utwórz inne zamówienie w ramach systemu połączonym z tym samym serwerem. | Na drugiej przeglądarce utworzono inne zamówienie i wprowadzono jego parametry. | zaliczony |
| 3 | Porównaj, czy zamówienia wprowadzane na jednym urządzeniu pojawiają się również na drugim. | Zaobserwowano, że na żadnej z przeglądarek nie wyświetlają się zamówienia wprowadzone w drugiej z nich. Po zamknięciu zamówień można jednak znaleźć oba w archiwum na obu mediach. | <span style="color: red;">niezaliczony</span> |

**uwagi**: System został stworzony pod działanie na tylko jednym urządzeniu - dane o zamówieniach zbierane są w pamięci podręcznej, a dopiero po ich zamknięciu trafiają do bazy danych. Możliwe, że zwiększa to jego wydajność, ale wyraźnie ogranicza uniwersalność zastosowania, co jest również ważnym czynnikiem.

## TC-TEASHOP-11-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-11-01
- **opis**: sprawdzenie przejrzystości komunikacji systemu z pracownikiem i informacji o powodzeniu bądź niepowodzeniu podjętych działań
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Wybierz wśród wykonanych testów te, w których czas oczekiwania na odpowiedź systemu był zauważalnie większy. | Zdecydowano się na powtórzenie przypadku testowego TC-TEASHOP-07-03. | zaliczony |
| 2 | Powtórz przypadki testowe. | Wprowadzono pięciokrotną treść wiersza Jana Morsztyna "Na krzyżyk na piersiach jednej panny" i wybrano opcję zapisania rezerwacji. Zauważono spowolnienie systemu wskutek wprowadzenia długiego ciągu znaków. | zaliczony |
| 3 | Zwracaj uwagę na obecność bądź nieobecność informacji zwrotnych. | Wybrano opcję zapisania rezerwacji. System przetwarzał polecenie ok. 3 s, nie podając żadnej informacji zwrotnej dotyczącej tego, czy zajmuje się jego wykonaniem. | <span style="color: red;">niezaliczony</span> |

**uwagi**: Powtórzono jeden z przypadków testowych, sprawdzając obecność informacji zwrotnej systemu w sytuacjach przetwarzania dłuższych poleceń - jest to tylko jeden przykład, jednak na nim nie zaobserwowano żadnego komunikatu. Poleca się sprawdzić również inne funkcjonalności na rzecz informowania użytkownika o przetwarzaniu przez system kosztowniejszych czasowo poleceń.

## TC-TEASHOP-12-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-12-01
- **opis**: sprawdzenie zachowania systemu przy natychmiastowym wprowadzeniu kilku różnych parametrów zamówienia
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, tester posiada zainstalowany wybrany program do automatyzacji kliknięć (np. Actiona na systemie Ubuntu)

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Kliknij "Nowe zamówienie". | Wybrano odpowiedni przycik. | zaliczony |
| 2 | Wprowadź dwa dowolne towary. | Wprowadzono dwa różne towary do utworzonego zamówienia. | zaliczony |
| 3 | Za pomocą systemu do automatyzacji kliknięć zaznacz status wyniesienia obu towarów oraz status opłacenia zamówienia - każdy w odstępie 0.5 s. | Zaobserwowano, że system ma problem z natychmiastowym przetworzeniem obu poleceń. Ikonki ze statusem wyniesienia zaczynają świecić na różne kolory. Po odświeżeniu strony wszystkie są nieodznaczone. | <span style="color: red;">niezaliczony</span> | 

**uwagi**: Twórca systemu zauważył problem z responsywnością systemu przy szybkich manipulacjach danymi, jednak zamiast go rozwiązać, wprowadził zabawny komunikat o przeciążeniu - co jest dobrą praktyką, ale pewnie lepszą byłoby spróbować rozwiązać problem.

## TC-TEASHOP-12-02

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-12-02
- **opis**: sprawdzenie, czy archiwum towarów ma zabezpieczenia na wypadek zbyt długiego czasu procesowania
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, tester posiada zainstalowany wybrany program do automatyzacji kliknięć (np. Actiona na systemie Ubuntu)

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | W pasku górnym kliknij "Magazyn". | Wybrano odpowiednią zakładkę. | zaliczony |
| 2 | Wprowadź dowolny nowy towar do bazy danych. | Wybrano opcję tworzenia towaru i wprowadzono jego parametry | zaliczony |
| 3 | Za pomocą narzędzia do automatyzacji kliknięć kliknij kilkukrotnie w odstępie czasu 0.5 s zapisanie wprowadzonego rodzaju towaru. | System wyświetlił dwa powiadomienia - jedno o sukcesie dodania towaru, drugie o tym, że towar o danej nazwie już istnieje w bazie. | zaliczony |

**uwagi**: brak

## TC-TEASHOP-12-03

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-12-03
- **opis**: sprawdzenie zachowania systemu przy kilkukrotnym kliknięciu zapisania rezerwacji
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, tester posiada zainstalowany wybrany program do automatyzacji kliknięć (np. Actiona na systemie Ubuntu)

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | W pasku górnym kliknij "Rezerwacje". | Wybrano odpowiednią zakładkę. | zaliczony |
| 2 | Utwórz nową rezerwację. | Wybrano opcję tworzenia rezerwacji. | zaliczony |
| 3 | Wprowadź odpowiednie parametry - imię, godzinę i datę oraz stolik. | Wprowadzono odpowiednie dane. | zaliczony |
| 4 | Za pomocą programu do automatyzacji kliknięć wykonaj kilkukrotne zapisanie rezerwacji w odstępie 0.5 s. | Wykonano dwukrotne zapisanie rezerwacji. Odkryto, że obie, o identycznych parametrach, zostały zapisane. | <span style="color: red;">niezaliczony</span> |

**uwagi**: System nie posiada zabezpieczenia na wypadek przypadkowego kilkukrotnego wprowadzenia tej samej rezerwacji poprzez kilkukrotne wciśnięcie przycisku zapisania.

## TC-TEASHOP-12-04

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-12-04
- **opis**: sprawdzenie, czy system posiada zabezpieczenia na wypadek kilkukrotnego wysłania zamówienia do archwium bądź przywrócenia go.
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, tester posiada zainstalowany wybrany program do automatyzacji kliknięć (np. Actiona na systemie Ubuntu)

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Stwórz zamówienie i wprowadź jego dowolne parametry. | Stworzono zamówienie i wprowadzono jeden towar | zaliczony |
| 2 | Za pomocą programu do automatyzacji kliknięć zamknij zamówienie kilkukrotnie w odstępie 0.5 s. | Wykonano zgodnie z instrukcją. | zaliczony |
| 3 | W pasku górnym wybierz "Archiwum". | Wybrano odpowiednią zakładkę. Zaobserwowano, że zamówienie zostało zapisane w archiwum dwukrotnie. | <span style="color: red;">niezaliczony</span> |
| 4 | Rozwiń zamknięte zamówienie i za pomocą programu do automatyzacji kliknięć przywróć zamówienie kilkukrotnie w odstępie 0.5 s. | Jedno z utworzonych zamówień przywrócono, klikając za pomocą programu trzykrotnie odpowiedni przycisk. Po powrocie na stronę główną zaobserwowano, że przywrócone zamówienie występuje w trzech kopiach. | <span style="color: red;">niezaliczony</span> |

**uwagi**: System nie posiada zabezpieczenia na wypadek kilkukrotnego zamknięcia oraz kilkukrotnego przywrócenia wybranego zamówienia z archiwum, tworząc duplikaty.

## TC-TEASHOP-14-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-14-01
- **opis**: sprawdzenie czasu przechowywania rezerwacji przez system
- **data wykonania**: 31.12.2024 / 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego i dwa tygodnie czasu

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Utwórz rezerwację z terminem dwóch tygodni od momentu jej wprowadzenia. | Dnia 31.12.2024 stworzono rezerwację z dwutygodniowym wyprzedzeniem, na 13.01.2025. | zaliczony |
| 2 | Dzień przed wprowadzoną datą sprawdź, czy rezerwacja wciąż jest przechowywana przez system. | Po dwóch tygodniach zaobserwowano, że rezerwacja wciąż znajduje się na liście. | zaliczony |

**uwagi**: brak

## TC-TEASHOP-15-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-15-01
- **opis**: weryfikacja bezpieczeństwa systemu związanego z autoryzacją pracowników
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: niezweryfikowany użytkownik ma dostęp do strony głównej

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Spróbuj wykonać jakiekolwiek działanie w systemie. | Po wprowadzeniu w przeglądarce adresu strony, wyskoczyło okienko logowania. Wykonanie żadnej akcji nie jest możliwe bez autoryzacji. Po zalogowaniu i odświeżeniu strony, wymagane jest ponowne logowanie. | zaliczony |

**uwagi**: brak

## TC-TEASHOP-16-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-16-01
- **opis**: sprawdzenie, czy nowo zatrudniony pracownik jest w stanie łatwo przyswoić funkcjonowanie systemu i wykonanie podstawowych akcji
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: dostęp do osoby, która nie miała styczności z testowanym systemem, umożliwienie jej dostępu do ekranu głównego

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Polecić osobie stworzyć zamówienie oraz wprowadzić jego zadane dowolne parametry, nie podając szczegółów, jak to zrobić. | Prośbę i polecenie przekazano nowej pracowniczce w trakcie szkolenia. | zaliczony |
| 2 | Polecić osobie stworzyć rezerwację. | Nowa pracowniczka poprawnie stworzyła rezerwację i zapisała ją nie będąc wcześniej instruowaną nt. obsługi systemu. | zaliczony |

**uwagi**: Potwierdzono przejrzystość stworzonego systemu.

- **opis**: sprawdzenie, czy tworzenie zamówienia umożliwia niezawodne wprowadzenie wszystkich potrzebnych danych
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Kliknij "Nowe zamówienie". | Kliknięto odpowiedni przycisk. | zaliczony |
| 2 | Ustaw wszystkie potrzebne parametry zamówienia, takie jak: towar, rodzaj sprzedaży, cenę, zniżkę oraz stolik - wprowadź w odpowiednio podpisane okienka. | Wybrano pierwszy dostępny towar z rozwijanej listy, wprowadzono zniżkę 5% na zamówienie oraz przypisano stolik "o2". | zaliczony |
| 3 | Dodaj kolejny towar do utworzonego zamówienia. | Z rozwijanej listy wybrano drugi dostępny towar. | zaliczony |
| 4 | Zaznacz, że zamówienie zostało już opłacone, a później również wyniesione i zamknięte. | Zaznaczono odpowiednie przyciski. | zaliczony |

**uwagi**: brak

## TC-TEASHOP-02-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-02-01
- **opis**: sprawdzenie, czy można modyfikować otwarte zamówienia
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, istnieje już utworzone zamówienie z kilkoma towarami

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Usuń jeden z towarów w zamówieniu. | Usunięto drugi z towarów w otwartym w poprzednim przypadku testowym zamówieniu. | zaliczony |
| 2 | Zmień drugi z towarów w zamówieniu na jakiś inny. | Wymieniono pierwszy towar na inny z rozwijanej listy. | zaliczony |
| 3 | Zmień rodzaj sprzedaży zmienionego towaru. | Zamieniono typ towaru z domyślnego "sztuka" na "gram" | zaliczony |
| 4 | Zmień zaznaczony stolik zamówienia. | Zmieniono stolik na "b3". | zaliczony |

**uwagi**: brak

## TC-TEASHOP-03-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-03-01
- **opis**: sprawdzenie, czy zachowanie systemu po przypisaniu zamówieniu stolika odpowiada wymaganiom - to znaczy, czy są one sortowane w odpowiedniej kolejności.
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, istnieje utworzonych kilka zamówień bez przypisanych stolików.

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Wprowadź nazwy kilku stolików zgodnie z przyjętą konwencją. | Wprowadzono do dwóch różnych stolików nazwy "m4" oraz "b7". | zaliczony |
| 2 | Przypisz po jednym stoliku w każdej sali. | Dodano również dwa nowe zamówienia i ustawiono ich nazwy jako "o9" oraz "s5". | zaliczony |
| 3 | W jednej z sal wprowadź więcej niż jeden stolik. | Dodano nowe zamówienie i przypisano mu stolik "o1" | zaliczony |

**uwagi**: brak

## TC-TEASHOP-04-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-04-01
- **opis**: sprawdzenie, czy archiwum dostępnych towarów funkcjonuje zgodnie z oczekiwaniami - czy szukanie towaru nie jest uciążliwe, a także czy możliwa jest modyfikacja listy.
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, istnieje otwarte zamówienie z wprowadzonym jednym towarem.

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Ręcznie zmień cenę wprowadzanego towaru w otwartym zamówieniu. | Zmieniono cenę wybranego towaru na 30 zł. | zaliczony |
| 2 | W pasku górnym kliknij "Magazyn". | Wybrano odpowiedni przycisk, przechodząc do listy towarów. | zaliczony |
| 3 | Zmodyfikuj cenę wybranego towaru. | Zmieniono nazwę towaru "akcesoria" w wersji "opakowanie" na 10 zł. | zaliczony |
| 4 | Wprowadź nowy towar, ustaw jego nazwę i cenę. | Wybrano opcję tworzenia nowego produktu, nazwano go "test" oraz wprowadzono cenę 2000 zł. | zaliczony |
| 5 | Wróć do ekranu głównego i dodaj do otwartego zamówienia utworzony wcześniej towar. | Dodano odpowiedni towar do zamówienia. | zaliczony |

**uwagi**: brak

## TC-TEASHOP-05-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-05-01
- **opis**: sprawdzenie funkcjonalności wprowadzania, modyfikacji i usuwania rezerwacji
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego.

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | W pasku górnym kliknij "Rezerwacje". | Wybrano odpowiedni przycisk. | zaliczony |
| 2 | Utwórz nową rezerwację. | Wybrano odpowiedni przycisk. | zaliczony |
| 3 | Wprowadź odpowiednie parametry - imię, godzinę i datę oraz stolik. | Wprowadzono imię, stolik, godzinę i datę - tą ostatnią na 2055 rok. | zaliczony |
| 4 | Zapisz rezerwację. | Zapisano rezerwację, która wyświetliła się na liście na samym końcu, odpowiednio posortowana chronologicznie. | zaliczony |
| 5 | Edytuj utworzoną wcześniej rezerwację, zmieć któreś z parametrów i zapisz ponownie. | Wybrano przycisk edycji rezerwacji i zmieniono datę na aktualny dzień z godzinnym wyprzedzeniem. Po zapisaniu stwierdzono ponowne poprawne posortowanie chronologiczne obecnych rezerwacji. | zaliczony |
| 6 | Usuń stworzoną rezerwację. | Wybrano przycisk edycji rezerwacji i usunięto ją. | zaliczony |

**uwagi**: brak

## TC-TEASHOP-06-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-06-01
- **opis**: sprawdzenie, czy w procesie dodawania i modyfikowania rezerwacji system w odpowiedni sposób je sortuje i układa na ekranie
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego.

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | W pasku górnym kliknij "Rezerwacje". | Wybrano odpowiedni przycisk. | zaliczony |
| 2 | Utwórz dwie rezerwacje w różnym czasie. | Stworzono dwie rezerwacje w dwa różne dni - najpierw późniejszą, potem wcześniejszą. | zaliczony |
| 3 | Sprawdź, czy zostały one posortowane chronologicznie. | Zaobserwowano poprawne sortowanie. | zaliczony |
| 4 | Zmodyfikuj późniejszą rezerwację, aby była ona wcześniej od tej drugiej. | Wybrano przycisk edycji późniejszej rezerwacji i zmieniono odpowiedni datę i godzinę. | zaliczony |
| 5 | Zapisz modyfikację. | Zapisano wykonaną modyfikację. | zaliczony |
| 6 | Sprawdź, czy system ponownie uporządkował rezerwacje. | Zaobserwowano ponowne poprawne posortowanie chronologiczne. | zaliczony |

**uwagi**: brak

## TC-TEASHOP-07-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-07-01
- **opis**: sprawdzenie zachowania systemu po wprowadzeniu niepoprawnej nazwy stolika w zamówieniu
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: orange;">częściowo zaliczony</span>

### Opis wykonania

**warunki wstępne**: autoryzowany użytkownik ma dostęp do ekranu głównego, istnieje utworzonych kilka zamówień bez przypisanych stolików.

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Utwórz kilka zamówień. | Utworzono trzy zamówienia. | zaliczony |
| 2 | Wprowadź nazwy kilku stolików zgodnie z przyjętą konwencją. | Dla dwóch z utworzonych zamówień wprowadzono nazwy "b304" oraz "m70". Zaobserwowano poprawne posortowanie zamówień oraz podświetlenie ich zgodnie z kolorem sali. | zaliczony |
| 3 | Wprowadź niepoprawną nazwę stolika. | Wprowadzono nazwę stolika, która jest przekopiowaną treścią "Pana Tadeusza". Cała treść została wprowadzona, po czym zaobserwowano gwałtowny spadek czasu odpowiedzi systemu. Stolik z nieprawidłową nazwą nie został posortowany ani podświetlony. | <span style="color: orange;">częściowo zaliczony</span> |

**uwagi**: System poprawnie rozpoznaje dopuszczalne nazwy stolików i odpowiedni jest sortuje, zauważono jednak, że pole nazwy stolika nie ma dopuszczalnego bufora znaków, pozwalając na wprowadzenie nielimitowanej ich ilości, co może w ekstremalnych przypadkach przełożyć się na gwałtowne pogorszenie wydajności funkcjonowania systemu.

## TC-TEASHOP-07-02

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-07-02
- **opis**: sprawdzenie, czy archiwum towarów ma wprowadzone zabezpieczenia na wypadek wprowadzania niewłaściwych wartości i przepełniania bufora znaków.
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | W pasku górnym kliknij "Magazyn". | Wybrano odpowiednią zakładkę. | zaliczony |
| 2 | Wprowadź nowy towar. | Wybrano opcję tworzenia nowego produktu. | zaliczony |
| 3 | Jako nazwę towaru wprowadź długi ciąg znaków | W odpowiednie pole przekopiowano wiersz Morsztyna "Do Kanikuły". Cała treść została dopuszczona. | <span style="color: red;">niezaliczony</span> |
| 4 | Jako cenę towaru wprowadź ciąg tekstowy. | Spróbowano wprowadzić ciąg liter, na co system nie pozwolił. | zaliczony |
| 5 | Wróć do ekranu głównego. | Powrócono do ekranu głównego. | zaliczony |
| 6 | Utwórz nowe zamówienie, używając stworzonego towaru. | Utworzono zamówienie, wybierając towar, którego nazwa jest barokowym wierszem. Zauważono wyraźny spadek czasu odpowiedzi systemu. | zaliczony |

**uwagi**: System nie posiada zabezpieczeń na wypadek przepełnienia pola nazwy towaru i zezwala na utworzenie nieograniczenie długiego ciągu znaków, co przekłada się na zauważalny spadek jego wydajności i wprowadza ryzyko awarii.

## TC-TEASHOP-07-03

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-07-03
- **opis**: sprawdzenie zabezpieczeń systemu rezerwacji przed wprowadzaniem niewłaściwych parametrów i przepełnienia bufora znaków
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | W pasku górnym kliknij "Rezerwacje". | Wybrano odpowiednią zakładkę. | zaliczony |
| 2 | Utwórz nową rezerwację. | Wybrano przycisk tworzenia rezerwacji. Zaobserwowano wyłączenie systemu i pokazywanie pustej strony. Po odczekaniu około minuty ponowiono próbę, obserwując poprawne wyświetlenie okienka dodawania rezerwacji. | <span style="color: red;">niezaliczony</span> |
| 3 | W którymś z pól wprowadź możliwie jak najdłuższy ciąg znaków. | W pole do uwag dotyczących zamówienia wprowadzono całą treść "Przedwiośnia" Stefana Żeromskiego, na co system pozwolił. Zaobserwowano gwałtowny spadek czasu odpowiedzi systemu. | <span style="color: red;">niezaliczony</span> |
| 4 | Zapisz rezerwację. | Ze względu na ryzyko awarii, nie zdecydowano się na zapisanie rezerwacji z błędnymi danymi | brak |

**uwagi**: System nie posiada zabezpieczeń na wypadek przepełnienia pól tekstowych przy tworzeniu rezerwacji i zezwala na utworzenie nieograniczenie długiego ciągu znaków, co przekłada się na zauważalny spadek jego wydajności i wprowadza ryzyko awarii.

## TC-TEASHOP-08-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-08-01
- **opis**: sprawdzenie, czy podczas zamykania zamówień wszystkie w odpowiedni sposób trafiają do archiwum i są sumowane zgodnie z oczekiwaniami
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Utwórz kilka zamówień, każde z kilkoma towarami. | Utworzono dwa różne zamówienia, z różnymi towarami, zaznaczając stolik, wyniesienie oraz odznaczając, że zostały opłacone. | zaliczony |
| 2 | Zamknij zamówienia. | Zamknięto oba. | zaliczony |
| 3 | W pasku górnym wybierz "Archiwum". | Wybrano odpowiednią zakładkę. | zaliczony |
| 4 | Sprawdź, czy zamknięte zamówienia znalazły się w archiwum, a także czy podsumowanie ceny zgadza się z wartością faktyczną. | Potwierdzono obecność obu zamówień i poprawne zsumowanie ich kwoty. | zaliczony |
| 5 | Kliknij przycisk "Przywróć" | Wybrano odpowiedni przycik. | zaliczony |
| 6 | Wróć do ekranu głównego i sprawdź, czy przywrócone zamówienie znajduje się na liście, wraz ze wszystkimi wprowadzonymi wcześniej parametrami. | Przywrócono oba zamówienia, które pojawiły się na ekranie głównym. Zniknęła jednak informacja o ich statusie opłacenia oraz stopniu przygotowania - jedynie stolik pozostał zaznaczony. | <span style="color: red;">niezaliczony</span> |

**uwagi**: Zaobserwowano, że przy przywracaniu zamówień z archiwum giną wszystkie informacje o nich poza listą zamówionych w ich ramach towarów. Może to być celowa architektura, mająca na celu zmniejszenie ilości przechowywanych informacji, jednak prawdopodobnie w niektórych przypadkach może wyraźnie brakować tej funkcjonalności.

## TC-TEASHOP-09-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-09-01
- **opis**: sprawdzenie, czy możliwe jest połączenie się z systemem na dwóch różnych urządzeniach/platformach, a także czy wprowadzane dane są odpowiednio odświeżane na obu
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego na dwóch różnych przeglądarkach internetowych

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Utwórz zamówienie z dowolnymi parametrami na jednym urządzeniu. | Utworzono odpowiednie zamówienie i wprowadzono kilka towarów. | zaliczony |
| 2 | Na drugim urządzeniu utwórz inne zamówienie w ramach systemu połączonym z tym samym serwerem. | Na drugiej przeglądarce utworzono inne zamówienie i wprowadzono jego parametry. | zaliczony |
| 3 | Porównaj, czy zamówienia wprowadzane na jednym urządzeniu pojawiają się również na drugim. | Zaobserwowano, że na żadnej z przeglądarek nie wyświetlają się zamówienia wprowadzone w drugiej z nich. Po zamknięciu zamówień można jednak znaleźć oba w archiwum na obu mediach. | <span style="color: red;">niezaliczony</span> |

**uwagi**: System został stworzony pod działanie na tylko jednym urządzeniu - dane o zamówieniach zbierane są w pamięci podręcznej, a dopiero po ich zamknięciu trafiają do bazy danych. Możliwe, że zwiększa to jego wydajność, ale wyraźnie ogranicza uniwersalność zastosowania, co jest również ważnym czynnikiem.

## TC-TEASHOP-11-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-11-01
- **opis**: sprawdzenie przejrzystości komunikacji systemu z pracownikiem i informacji o powodzeniu bądź niepowodzeniu podjętych działań
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Wybierz wśród wykonanych testów te, w których czas oczekiwania na odpowiedź systemu był zauważalnie większy. | Zdecydowano się na powtórzenie przypadku testowego TC-TEASHOP-07-03. | zaliczony |
| 2 | Powtórz przypadki testowe. | Wprowadzono pięciokrotną treść wiersza Jana Morsztyna "Na krzyżyk na piersiach jednej panny" i wybrano opcję zapisania rezerwacji. Zauważono spowolnienie systemu wskutek wprowadzenia długiego ciągu znaków. | zaliczony |
| 3 | Zwracaj uwagę na obecność bądź nieobecność informacji zwrotnych. | Wybrano opcję zapisania rezerwacji. System przetwarzał polecenie ok. 3 s, nie podając żadnej informacji zwrotnej dotyczącej tego, czy zajmuje się jego wykonaniem. | <span style="color: red;">niezaliczony</span> |

**uwagi**: Powtórzono jeden z przypadków testowych, sprawdzając obecność informacji zwrotnej systemu w sytuacjach przetwarzania dłuższych poleceń - jest to tylko jeden przykład, jednak na nim nie zaobserwowano żadnego komunikatu. Poleca się sprawdzić również inne funkcjonalności na rzecz informowania użytkownika o przetwarzaniu przez system kosztowniejszych czasowo poleceń.

## TC-TEASHOP-12-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-12-01
- **opis**: sprawdzenie zachowania systemu przy natychmiastowym wprowadzeniu kilku różnych parametrów zamówienia
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, tester posiada zainstalowany wybrany program do automatyzacji kliknięć (np. Actiona na systemie Ubuntu)

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Kliknij "Nowe zamówienie". | Wybrano odpowiedni przycik. | zaliczony |
| 2 | Wprowadź dwa dowolne towary. | Wprowadzono dwa różne towary do utworzonego zamówienia. | zaliczony |
| 3 | Za pomocą systemu do automatyzacji kliknięć zaznacz status wyniesienia obu towarów oraz status opłacenia zamówienia - każdy w odstępie 0.5 s. | Zaobserwowano, że system ma problem z natychmiastowym przetworzeniem obu poleceń. Ikonki ze statusem wyniesienia zaczynają świecić na różne kolory. Po odświeżeniu strony wszystkie są nieodznaczone. | <span style="color: red;">niezaliczony</span> | 

**uwagi**: Twórca systemu zauważył problem z responsywnością systemu przy szybkich manipulacjach danymi, jednak zamiast go rozwiązać, wprowadził zabawny komunikat o przeciążeniu - co jest dobrą praktyką, ale pewnie lepszą byłoby spróbować rozwiązać problem.

## TC-TEASHOP-12-02

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-12-02
- **opis**: sprawdzenie, czy archiwum towarów ma zabezpieczenia na wypadek zbyt długiego czasu procesowania
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, tester posiada zainstalowany wybrany program do automatyzacji kliknięć (np. Actiona na systemie Ubuntu)

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | W pasku górnym kliknij "Magazyn". | Wybrano odpowiednią zakładkę. | zaliczony |
| 2 | Wprowadź dowolny nowy towar do bazy danych. | Wybrano opcję tworzenia towaru i wprowadzono jego parametry | zaliczony |
| 3 | Za pomocą narzędzia do automatyzacji kliknięć kliknij kilkukrotnie w odstępie czasu 0.5 s zapisanie wprowadzonego rodzaju towaru. | System wyświetlił dwa powiadomienia - jedno o sukcesie dodania towaru, drugie o tym, że towar o danej nazwie już istnieje w bazie. | zaliczony |

**uwagi**: brak

## TC-TEASHOP-12-03

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-12-03
- **opis**: sprawdzenie zachowania systemu przy kilkukrotnym kliknięciu zapisania rezerwacji
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, tester posiada zainstalowany wybrany program do automatyzacji kliknięć (np. Actiona na systemie Ubuntu)

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | W pasku górnym kliknij "Rezerwacje". | Wybrano odpowiednią zakładkę. | zaliczony |
| 2 | Utwórz nową rezerwację. | Wybrano opcję tworzenia rezerwacji. | zaliczony |
| 3 | Wprowadź odpowiednie parametry - imię, godzinę i datę oraz stolik. | Wprowadzono odpowiednie dane. | zaliczony |
| 4 | Za pomocą programu do automatyzacji kliknięć wykonaj kilkukrotne zapisanie rezerwacji w odstępie 0.5 s. | Wykonano dwukrotne zapisanie rezerwacji. Odkryto, że obie, o identycznych parametrach, zostały zapisane. | <span style="color: red;">niezaliczony</span> |

**uwagi**: System nie posiada zabezpieczenia na wypadek przypadkowego kilkukrotnego wprowadzenia tej samej rezerwacji poprzez kilkukrotne wciśnięcie przycisku zapisania.

## TC-TEASHOP-12-04

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-12-04
- **opis**: sprawdzenie, czy system posiada zabezpieczenia na wypadek kilkukrotnego wysłania zamówienia do archwium bądź przywrócenia go.
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: red;">niezaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego, tester posiada zainstalowany wybrany program do automatyzacji kliknięć (np. Actiona na systemie Ubuntu)

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Stwórz zamówienie i wprowadź jego dowolne parametry. | Stworzono zamówienie i wprowadzono jeden towar | zaliczony |
| 2 | Za pomocą programu do automatyzacji kliknięć zamknij zamówienie kilkukrotnie w odstępie 0.5 s. | Wykonano zgodnie z instrukcją. | zaliczony |
| 3 | W pasku górnym wybierz "Archiwum". | Wybrano odpowiednią zakładkę. Zaobserwowano, że zamówienie zostało zapisane w archiwum dwukrotnie. | <span style="color: red;">niezaliczony</span> |
| 4 | Rozwiń zamknięte zamówienie i za pomocą programu do automatyzacji kliknięć przywróć zamówienie kilkukrotnie w odstępie 0.5 s. | Jedno z utworzonych zamówień przywrócono, klikając za pomocą programu trzykrotnie odpowiedni przycisk. Po powrocie na stronę główną zaobserwowano, że przywrócone zamówienie występuje w trzech kopiach. | <span style="color: red;">niezaliczony</span> |

**uwagi**: System nie posiada zabezpieczenia na wypadek kilkukrotnego zamknięcia oraz kilkukrotnego przywrócenia wybranego zamówienia z archiwum, tworząc duplikaty.

## TC-TEASHOP-14-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-14-01
- **opis**: sprawdzenie czasu przechowywania rezerwacji przez system
- **data wykonania**: 31.12.2024 / 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: zautoryzowany użytkownik ma dostęp do ekranu głównego i dwa tygodnie czasu

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Utwórz rezerwację z terminem dwóch tygodni od momentu jej wprowadzenia. | Dnia 31.12.2024 stworzono rezerwację z dwutygodniowym wyprzedzeniem, na 13.01.2025. | zaliczony |
| 2 | Dzień przed wprowadzoną datą sprawdź, czy rezerwacja wciąż jest przechowywana przez system. | Po dwóch tygodniach zaobserwowano, że rezerwacja wciąż znajduje się na liście. | zaliczony |

**uwagi**: brak

## TC-TEASHOP-15-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-15-01
- **opis**: weryfikacja bezpieczeństwa systemu związanego z autoryzacją pracowników
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: niezweryfikowany użytkownik ma dostęp do strony głównej

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Spróbuj wykonać jakiekolwiek działanie w systemie. | Po wprowadzeniu w przeglądarce adresu strony, wyskoczyło okienko logowania. Wykonanie żadnej akcji nie jest możliwe bez autoryzacji. Po zalogowaniu i odświeżeniu strony, wymagane jest ponowne logowanie. | zaliczony |

**uwagi**: brak

## TC-TEASHOP-16-01

### Informacje ogólne

- **identyfikator przypadku testowego**: TC-TEASHOP-16-01
- **opis**: sprawdzenie, czy nowo zatrudniony pracownik jest w stanie łatwo przyswoić funkcjonowanie systemu i wykonanie podstawowych akcji
- **data wykonania**: 12.01.2025
- **tester**: Krzysztof Czarnowus
- **status**: <span style="color: green;">zaliczony</span>

### Opis wykonania

**warunki wstępne**: dostęp do osoby, która nie miała styczności z testowanym systemem, umożliwienie jej dostępu do ekranu głównego

**kroki**:
| nr kroku | opis kroku | wynik | status testu |
|----------|------------|-------|--------------|
| 1 | Polecić osobie stworzyć zamówienie oraz wprowadzić jego zadane dowolne parametry, nie podając szczegółów, jak to zrobić. | Prośbę i polecenie przekazano nowej pracowniczce w trakcie szkolenia. | zaliczony |
| 2 | Polecić osobie stworzyć rezerwację. | Nowa pracowniczka poprawnie stworzyła rezerwację i zapisała ją nie będąc wcześniej instruowaną nt. obsługi systemu. | zaliczony |

**uwagi**: Potwierdzono przejrzystość stworzonego systemu.
