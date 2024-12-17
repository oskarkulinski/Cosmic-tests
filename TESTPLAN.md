# Plan Testów zgodny z normą ISO 29119

## 1. Identyfikator

TP-COSMIC-001

## 2. Wprowadzenie 
Celem tego planu testowania jest ~~znalezienie bugów~~ zdefiniowanie podejścia, 
narzędzi, zasobów, harmonogramu i aktywności niezbędnych do weryfikacji
i walidacji COSMIC. Jest on środowiskiem graficznym dla system Linux, 
stworzonym by uprościć i zmodernizować korzystanie z systemu Linux.

## 3. Obiekt testowania   
COSMIC w najnowszej wersji dostępnej.   
Kluczowe funkcjonalności:   
- edytor tekstu
- eksplorator plików
- sklep aplikacji
- ustawienia systemowe
- terminal

## 4. Funkcjonalności do przetestowania
- edytor tekstu - TC-EDIT
- eksplorator plików -  TC-FILE
- sklep aplikacji - TC-STOR
- ustawienia systemowe - TC-SETT
- terminal - TC-TERM
- polska wersja językowa - TC-COSM
- aplety - TC-APPL

## 5. Funkcjonalności, które nie będą testowane
- obsługa okien
- kompozytor
- ikony
- zrzuty ekranu
- witacz

## 6. Podejścia
Techniki:   
- testy białoskrzynkowe
- testy czarnoskrzynkowe
- testy jednostkowe
- testy systemowe, całego oprogramowania   

Narzędzia i środowisko:
- w celu automatyzacji testów Sikuli, KatalonStudio, PyAutoGui
- do testów jednostkowych Rust
- Linux

## 7. Kryteria akceptacji lub odrzucenia
Akceptacja:
- zrealizowane testy dla wszystkich przypadków testowych
- zweryfikowane wszystkie wymagania
- 90% testów zakończonych wynikiem pozytywnym

Odrzucenie:
- brak zweryfikowanych wszystkich wymagań
- niezrealizowanie testów dla niektórych przypadków testowych


## 8. Kryteria zawieszenia i wymagania wznowienia
- testy zostaną zawieszone w przypadku krytycznych problemów ze środowiskiem (na przykład awaria sprzętowa)
- testy zostaną zawieszone w przypadku nieprzewidzianej sytuacji geopolitycznej stwarzającej znaczące zagrożenie dla życia lub zdrowia 
zespołu testowego
- testy zostaną wznowione po rozwiązaniu krytycznych problemow ze środowiskiem
- testy zostaną wznowione po uspokojeniu się sytuacji geopolitycznej 

## 9. Rezultaty testowanie
- dokumentacja testowania w formacie Markdown
- logi z wykonania testów 
- raport podsumowujący testy, zawierający metryki i analizę defektów


## 10. Zadania testowania
- przygotowanie przypadków testowych
- wykonanie testów
- sporządzenie dokumentacji testów

## 11. Potrzeby środowiskowe
- Sprzęt:
    - komputer z procesorem o architekturze x86

- Oprogramowanie:
    - Zainstalowany system POP!_OS 24.04
    - Dodane repozytorium popdev:master
    - Zaaktualizowany system operacyjny

## 12. Odpowiedzialności
- Oskar - testy jednostkowe, testy funkcjonalne
- Wieńczysław - testy jednostkowe, testy funkcjonalne
- Filip - testy funkcjonalne, testy systemowe
- Kajetan - testy funkcjonalne, testy systemowe

## 13. Harmonogram
1. 23.11 - 29.11 - przygotowanie przypadków testowych wysokopoziomowe
2. 30.11 - 6.12 - przygotowanie przypadków testowych niskopoziomowe
3. 7.12 - 13.12 - wykonanie testów - tydzień 1
4. 14.12 - 20.12 - wykonanie testów - tydzień 2
5. 4.01 - 10.01 - wykonanie testów - tydzień 3
6. 11.01 - 17.01 - wykonanie testów - tydzień 4
7. 18.01 - 24.01 - przygotowanie finalnego raportu
 i podsumowanie testów

 ## 14. Zagrożenia i ich minimalizacja
 1. COSMIC jest pisany w Rust, więc wystąpienie błędów jest mniej prawdopodobne niż zwykle
    - Przeprowadzanie gruntownych, dogłębnych testów 
    - Wpływ średni
    - Prawdopodobieństwo wysokie 
 2. Na razie niskie umiejętności testerskie mogą nie sprostać tak skomplikowanemu projektowi
    - Poprawa umiejętności testerskich, zawężenie testów do jedynie części projektu
    - Wpływ średni
    - Prawdopodobieństwo średnie
 3. Brak pełnej dokumentacji wynikający z wersji alfa projektu
    - Zapoznanie się z dostępną dokumentacją, aktywna komunikacja z developerami projektu
    - Wpływ niski
    - Prawdopodobieństwo wysokie
 4. Wysoka trudność przetestowania pewnych elementów aplikacji
    - Poświęcenie większego nakładu pracy do tych elementów jeśli jest to wymagane lub skupienie się na elementach prostszych do testowania
    - Wpływ niski
    - Prawdopodobieństwo średnie
 5. Zdarzenie losowe (np. Gorączka Zachodniego Nilu, wojna nuklearna)
    - Zadbanie o zdrowie, przyjmowanie dużej ilości witamin i środków uodparniających na promieniowanie
    - Ryzyko średnie
    - Wpływ średni
 6. Natłok obowiązków związanych z uczelnią lub pracą
    - Rozłożenie pracy tak aby każdy w miarę dawał radę
    - Ryzyko wysokie
    - Wpływ niski
 7. Brak narzędzi do automatyzacji testów
    - Zaznajomienie się z takimi narzędziami i innymi technologiami do testowania
    - Wpływ średni
    - Prawdopodobieństwo średnie
 8. Duża liczba aktualizacji
    - Bycie na bieżąco z każdą zmianą, kontakt z developerami projektu
    - Wpływ niski
    - Prawdopodobieństwo wysokie
 9. Szybko rozwijający się projekt może doprowadzić do rozjeżdżania się planów i przypadków testowych
    - „Napisanie przypadków testowych wysokiego poziomu i przeniesienie szczegółów, które mogą się zmieniać do danych testowych”
    - Wpływ średni
    - Prawdopodobieństwo średnie

## 15. Zatwierdzenie
 Plan testów zostanie zatwierdzony demokratycznie większością 3/4 głosów przez zespół, oraz przez prowadzącego zajęcia, po zapoznaniu się z rezultatami testowania.

## 16. Repozytorium 
https://github.com/oskarkulinski/Cosmic-tests