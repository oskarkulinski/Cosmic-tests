# Plan Testów zgodny z normą ISO 29119

## 1. Wprowadzenie
### Cel testów 
~~Znalezienie bugów~~ Zapewnienie niezawodności, jakości i zgodności oprogramowania z wymaganiami.
### Kontekst biznesowy oprogramowania
COSMIC jest środowiskiem graficznym, które ma na celu unowocześnienie i zwiększenie komfortu pracy użytkowników w systemie Linux. Jest tworzony przez firmę System76, która planuje w przyszłości instalować COSMIC na sprzedawanych przez siebie laptopach, by zwiększyć ich atrakcyjność dla potencjalnych konsumentów. Grupą docelową są użytkownicy systemu Linux poszukujący nowoczesnego i dostosowanego do ich potrzeb środowiska graficznego, przede wszystkim profesjonalistów i inżynierów. COSMIC tworzony jest w języku programowania Rust. 
### Zakres testów
Testowane będą aplikacje dostarczane przez COSMIC (edytor tekstu, eksplorator plików, sklep aplikacji, edytor ustawień, terminal), applety, oraz polska wersja językowa.   

Skupimy się testach funkcjonalnych, zarówno białoskrzynkowych jak i czarnoskrzynkowych. Przeprowadzimy przede wszystkim testy jednostkowe i systemowe.
## 2. Cele i kryteria testów
### Kryteria wejścia
- Zainstalowany system POP!_OS 24.04
- Dodane repozytorium popdev:master
- Zaaktualizowany system operacyjny
### Kryteria wyjścia
- Koniec semestru
- Spełnione wszystkie wymagania
- Upewnienie się, że wszystkie kluczowe komponenty zostały przetestowane zgodnie z planem testów
- Wszystkie zidentyfikowane błędy zostały zreprodukowane i zgłoszone

### Kryteria akceptacji testów
- ?????

## 3. Strategia testowania
W pierwszej kolejności skupiać będziemy się na:
- testach jednostkowych, których niedobór został zgłoszony przez twórców oprogramowania.
- testach funkcjonalnych, przede wszystkim manualnych.
- edytorze tekstu
- eksploratorze plików
- ustawieniach systemowych
- appletach
- polskiej wersji językowej

W drugiej kolejności skupimy się na:
- automatycznych testach funkcjonalnych
- sklepie COSMIC
- terminalu
- testach regresyjnych

Do automatyzacji testów skorzystamy z narzędzi takich jak Sikuli, KatalonStudio, PyAutoGui.

## 4. Harmonogram i zasoby
Tygodnie:   
 1. Testy ustawień, edytora tekstu i polskiej wersji językowej, testy jednostkowe 
 2. Kontynuacja tygodnia pierwszego, eksplorator plików, rozpoczęcie testowania appletów
 3. Dalsze testowanie appletów, próby automatyzacji testów, testy jednostkowe
 4. Testy sklepu, terminala, potencjalnie testy regresyjne

Podział ról:
Podział ról będzie dynamicznie zmieniany zależnie od aktualnych priorytetów i umiejętności członków zespołu. Nie chcemy sztywnego przypisania ról, żeby każdy miał okazję nauczyć się wielu typów testowania.   

Wstępny podział ról:   
Oskar - testy jednostkowe   
Wieńczysław - testy jednostkowe, testy funkcjonalne   
Filip - testy funkcjonalne   
Kajetan - testy funkcjonalne

## 5. Zarządzanie ryzykiem
