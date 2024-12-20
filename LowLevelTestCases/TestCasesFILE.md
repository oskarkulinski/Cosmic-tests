# Przypadki testowe dla COSMIC File Explorer

## 1. LC-FILE-001: Weryfikacja poprawnego utworzenia nowego pliku tekstowego
**Cel:** Sprawdzić, czy użytkownik może utworzyć nowy plik tekstowy.

**Warunki wstępne:**  
- Użytkownik musi posiadać uprawnienia do zapisu w katalogu, w którym ma być utworzony nowy plik.

**Kroki:**  
1. Otworzyć File Explorer.  
2. Przejść do katalogu, w którym ma zostać utworzony nowy plik.  
3. Kliknąć prawym przyciskiem myszy i wybrać opcję "Nowy plik tekstowy".  
4. Wpisać nazwę pliku i nacisnąć Enter.

**Oczekiwany wynik:**  
- Nowy plik tekstowy powinien zostać utworzony w wybranej lokalizacji i wyświetlony w interfejsie.

**Scenariusz alternatywny:**  
- **Brak uprawnień do zapisu:** System powinien wyświetlić komunikat o błędzie, informujący użytkownika o braku uprawnień. Plik tekstowy nie powinien zostać utworzony.

---

## 2. LC-FILE-002: Weryfikacja poprawnego usunięcia pliku tekstowego
**Cel:** Sprawdzić, czy użytkownik może usunąć plik tekstowy.

**Warunki wstępne:**  
- Użytkownik musi posiadać uprawnienia do zapisu w katalogu, w którym znajduje się plik.  
- Plik tekstowy musi istnieć.

**Kroki:**  
1. Otworzyć File Explorer.  
2. Znaleźć plik tekstowy, który ma zostać usunięty.  
3. Kliknąć prawym przyciskiem myszy i wybrać opcję "Usuń".  
4. Potwierdzić operację w wyświetlonym komunikacie.

**Oczekiwany wynik:**  
- Plik tekstowy powinien zostać usunięty z wybranego katalogu.

**Scenariusz alternatywny:**  
- **Brak uprawnień do zapisu:** System powinien wyświetlić komunikat o błędzie, informujący użytkownika o braku uprawnień. Plik tekstowy powinien pozostać w katalogu.

---

## 3. LC-FILE-003: Weryfikacja możliwości otworzenia dowolnego katalogu z uprawnieniami do odczytu
**Cel:** Sprawdzić, czy użytkownik może otworzyć dowolny katalog z uprawnieniami do odczytu.

**Warunki wstępne:**  
- Katalog musi istnieć i być dostępny dla użytkownika z uprawnieniami do odczytu.

**Kroki:**  
1. Otworzyć File Explorer.  
2. Znaleźć katalog, który użytkownik chce otworzyć.  
3. Dwukrotnie kliknąć ikonę katalogu lub wybrać "Otwórz" z menu kontekstowego.

**Oczekiwany wynik:**  
- Katalog powinien zostać otwarty i zawartość powinna być widoczna w interfejsie.

**Scenariusz alternatywny:**  
- **Brak uprawnień do odczytu:** System powinien wyświetlić komunikat o błędzie, informujący użytkownika o braku uprawnień. Katalog nie powinien zostać otwarty, a jego zawartość powinna pozostać niedostępna.

---

## 4. LC-FILE-004: Weryfikacja możliwości sortowania wyświetlanych plików
**Cel:** Sprawdzić, czy użytkownik może sortować wyświetlane pliki według różnych kryteriów (nazwa, data, rozmiar) oraz w sposób odwrotny.

**Warunki wstępne:**  
- Katalog powinien zawierać wiele plików o różnych nazwach, datach utworzenia i rozmiarach.

**Kroki:**  
1. Otworzyć File Explorer.  
2. Przejść do katalogu zawierającego pliki.  
3. Kliknąć nagłówek kolumny (np. "Nazwa", "Data", "Rozmiar"), aby posortować pliki według wybranego kryterium.  
4. Kliknąć ponownie, aby zmienić kolejność sortowania na odwrotną.

**Oczekiwany wynik:**  
- Pliki powinny zostać posortowane zgodnie z wybranym kryterium i w wybranej kolejności.

**Scenariusz alternatywny:**  
- **Błąd w odczycie metadanych plików:** Jeśli metadane (np. data utworzenia) są niedostępne, system powinien pominąć te pliki w sortowaniu lub wyświetlić odpowiedni komunikat.

---

## 5. LC-FILE-005: Weryfikacja poprawnego otworzenia istniejącego pliku tekstowego
**Cel:** Sprawdzić, czy użytkownik może otworzyć istniejący plik tekstowy.

**Warunki wstępne:**  
- Plik tekstowy musi istnieć i być dostępny dla użytkownika z uprawnieniami do odczytu.

**Kroki:**  
1. Otworzyć File Explorer.  
2. Znaleźć plik tekstowy, który użytkownik chce otworzyć.  
3. Dwukrotnie kliknąć ikonę pliku tekstowego lub wybrać "Otwórz" z menu kontekstowego.

**Oczekiwany wynik:**  
- Plik tekstowy powinien zostać otwarty w domyślnym edytorze tekstu.

**Scenariusz alternatywny:**  
- **Brak uprawnień do odczytu:** System powinien wyświetlić komunikat o błędzie, informujący użytkownika o braku uprawnień. Plik nie powinien zostać otwarty.  
- **Plik jest uszkodzony lub niedostępny:** System powinien wyświetlić komunikat o błędzie, informujący użytkownika o problemach z plikiem.
