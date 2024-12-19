# Przypadki testowe dla COSMIC File Explorer

## 1. LC-FILE-001: Weryfikacja możliwości utworzenia nowego katalogu
**Cel:** Sprawdzić, czy użytkownik może utworzyć nowy katalog.

**Warunki wstępne:**  
- Użytkownik musi posiadać uprawnienia do zapisu w katalogu, w którym ma być utworzony nowy katalog.

**Kroki:**  
1. Otworzyć File Explorer.  
2. Przejść do katalogu, w którym ma zostać utworzony nowy katalog.  
3. Kliknąć prawym przyciskiem myszy i wybrać opcję "Nowy katalog".  
4. Wpisać nazwę katalogu i nacisnąć Enter.

**Oczekiwany wynik:**  
- Nowy katalog powinien zostać utworzony w wybranej lokalizacji i wyświetlony w interfejsie.

**Scenariusz alternatywny (Brak uprawnień do zapisu):**
- System powinien wyświetlić komunikat o błędzie, informujący użytkownika o braku uprawnień do zapisu w danej lokalizacji.  
- Nowy katalog nie powinien zostać utworzony.

---

## 2. LC-FILE-002: Weryfikacja możliwości przeniesienia pliku do innego katalogu
**Cel:** Sprawdzić, czy użytkownik może przenieść plik do innego katalogu.

**Warunki wstępne:**  
- Użytkownik musi posiadać uprawnienia do zapisu w docelowym katalogu i odczytu w źródłowym katalogu.  
- Plik źródłowy musi istnieć.

**Kroki:**  
1. Otworzyć File Explorer.  
2. Znaleźć plik, który ma zostać przeniesiony.  
3. Przeciągnąć plik do docelowego katalogu lub użyć opcji "Wytnij" i "Wklej".  

**Oczekiwany wynik:**  
- Plik powinien zostać usunięty z katalogu źródłowego i pojawić się w katalogu docelowym.

**Scenariusz alternatywny 1 (Brak uprawnień do zapisu w docelowym katalogu):** 
- System powinien wyświetlić komunikat o błędzie, informujący użytkownika o braku uprawnień do zapisu w docelowym katalogu.  
- Plik powinien pozostać w katalogu źródłowym.


**Scenariusz alternatywny 2 (Brak uprawnień do odczytu w źródłowym katalogu):**  
- Plik nie będzie widoczny w katalogu źródłowym lub dostępny do przeniesienia.  
- System powinien wyświetlić komunikat o błędzie, informujący użytkownika o braku uprawnień do odczytu w źródłowym katalogu.

---

## 3. LC-FILE-003: Weryfikacja możliwości kopiowania pliku do innego katalogu
**Cel:** Sprawdzić, czy użytkownik może skopiować plik do innego katalogu.

**Warunki wstępne:**  
- Użytkownik musi posiadać uprawnienia do zapisu w docelowym katalogu i odczytu w źródłowym katalogu.  
- Plik źródłowy musi istnieć.

**Kroki:**  
1. Otworzyć File Explorer.  
2. Znaleźć plik, który ma zostać skopiowany.  
3. Kliknąć prawym przyciskiem myszy i wybrać opcję "Kopiuj".  
4. Przejść do docelowego katalogu i kliknąć "Wklej".

**Oczekiwany wynik:**  
- Plik powinien pozostać w katalogu źródłowym i jednocześnie pojawić się w katalogu docelowym.

**Scenariusz alternatywny 1 (Brak uprawnień do zapisu w docelowym katalogu):**  
- System powinien wyświetlić komunikat o błędzie, informujący użytkownika o braku uprawnień do zapisu w docelowym katalogu.  
- Plik nie powinien zostać skopiowany do katalogu docelowego, ale powinien pozostać w katalogu źródłowym.


**Scenariusz alternatywny 2 (Brak uprawnień do odczytu w źródłowym katalogu):**  
- Plik nie będzie widoczny w katalogu źródłowym lub dostępny do skopiowania.  
- System powinien wyświetlić komunikat o błędzie, informujący użytkownika o braku uprawnień do odczytu w źródłowym katalogu.

---

## 4. LC-FILE-004: Weryfikacja możliwości zmiany nazwy pliku lub katalogu
**Cel:** Sprawdzić, czy użytkownik może zmienić nazwę istniejącego pliku lub katalogu.

**Warunki wstępne:**  
- Użytkownik musi posiadać uprawnienia do zapisu w katalogu, w którym znajduje się plik lub katalog.  
- Plik lub katalog musi istnieć.

**Kroki:**  
1. Otworzyć File Explorer.  
2. Znaleźć plik lub katalog do zmiany nazwy.  
3. Kliknąć prawym przyciskiem myszy i wybrać "Zmień nazwę".  
4. Wprowadzić nową nazwę i nacisnąć Enter.

**Oczekiwany wynik:**  
- Nazwa pliku lub katalogu powinna zostać zmieniona i poprawnie wyświetlona w interfejsie.


**Scenariusz alternatywny 1 (Brak uprawnień do zapisu w katalogu):**  
- System powinien wyświetlić komunikat o błędzie, informujący użytkownika o braku uprawnień do zmiany nazwy pliku lub katalogu.  
- Nazwa pliku lub katalogu powinna pozostać niezmieniona.

**Scenariusz alternatywny 2 (Plik lub katalog jest otwarty w innym programie):**  
- System powinien wyświetlić komunikat o błędzie, informujący użytkownika, że plik lub katalog jest obecnie używany i nie można zmienić jego nazwy.  
- Nazwa pliku lub katalogu powinna pozostać niezmieniona.

---

## 5. LC-FILE-005: Weryfikacja możliwości wyszukiwania plików lub katalogów według nazwy
**Cel:** Sprawdzić, czy użytkownik może wyszukać pliki lub katalogi na podstawie nazwy.

**Warunki wstępne:**  
- System musi zawierać pliki lub katalogi z nazwami pasującymi do wyszukiwanego wzorca.

**Kroki:**  
1. Otworzyć File Explorer.  
2. Wpisać nazwę pliku lub katalogu w pasku wyszukiwania.  
3. Nacisnąć Enter i przeglądać wyniki.

**Oczekiwany wynik:**  
- Wyniki wyszukiwania powinny wyświetlić wszystkie pliki i katalogi pasujące do wpisanej nazwy.

**Scenariusz alternatywny (Brak wyników wyszukiwania):** 
- System powinien wyświetlić komunikat informujący, że nie znaleziono plików ani katalogów pasujących do podanej nazwy.
