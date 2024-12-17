# Niskopoziomowe Przypadki Testowe dla Edytora Tekstowego "Cosmic"

## 1. TC-EDIT-01: Weryfikacja możliwości otwarcia pliku tekstowego
**Cel:** Sprawdzić, czy użytkownik może otworzyć dowolny plik tekstowy.

**Warunki wstępne:**
- Oprogramowanie "Cosmic" musi być zainstalowane na systemie Linux.
- Plik tekstowy (np. .txt, .cpp, .py) musi istnieć w dostępnej lokalizacji na systemie plików.
- Użytkownik musi posiadać odpowiednie uprawnienia do odczytu pliku.

**Kroki:**
1. Uruchomić edytor tekstowy "Cosmic".
2. Kliknąć na opcję "Plik" w górnym menu.
3. Wybrać opcję "Otwórz Plik...".
4. W oknie dialogowym otwierania pliku, wybrać plik tekstowy (np. `sample.txt`).
5. Kliknąć na przycisk "Otwórz" (albo otworzyć klikając dwa razy).

**Oczekiwany wynik:**
- Edytor powinien otworzyć plik bez błędów.
- Zawartość pliku powinna być wyświetlana poprawnie w edytorze tekstowym.

**Scenariusz 2 (Użytkownik NIE ma uprawnień do zapisu w katalogu):**
- Po próbie otwarcia pliku, system powinien wyświetlić komunikat o błędzie, informujący o braku uprawnień do oczytu pliku.
- Plik nie powinien zostać odczytany.

---

## 2. TC-EDIT-02: Weryfikacja możliwości zapisania otwartego pliku tekstowego
**Cel:** Sprawdzić, czy użytkownik może zapisać otwarty plik tekstowy w dowolnym katalogu, do którego ma uprawnienia w systemie operacyjnym.

**Warunki wstępne:**
- Oprogramowanie "Cosmic" musi być uruchomione.
- Użytkownik musi mieć otwarty plik tekstowy (np. `sample.txt`) w edytorze.
- Użytkownik musi mieć uprawnienia do zapisu w wybranym katalogu.

**Kroki:**
1. Upewnić się, że plik tekstowy jest otwarty w edytorze.
2. Kliknąć na opcję "Plik" w górnym menu.
3. Wybrać "Zapisz jako".
4. W oknie dialogowym zapisu pliku, wskazać nowy katalog lub ścieżkę do istniejącego katalogu.
5. Wpisać nazwę pliku i kliknąć przycisk "Zapisz".

**Oczekiwany wynik:**
- Plik powinien zostać zapisany w wybranym katalogu bez błędów.
- Zawartość pliku powinna być taka sama, jak przed zapisaniem.
- Jeżeli użytkownik nie ma uprawnień do zapisu w wybranym katalogu, wyświetlony zostanie komunikat o błędzie.

**Scenariusz 2 (Użytkownik NIE ma uprawnień do zapisu w katalogu):**
- Po próbie zapisania pliku, system powinien wyświetlić komunikat o błędzie, informujący o braku uprawnień do zapisu w wybranym katalogu
- Plik nie powinien zostać zapisany, a katalog nie powinien zmienić swojego stanu.

---

## 3. TC-EDIT-03: Weryfikacja możliwości utworzenia nowego pliku tekstowego
**Cel:** Sprawdzić, czy użytkownik może utworzyć nowy, pusty plik tekstowy w edytorze.

**Warunki wstępne:**
- Oprogramowanie "Cosmic" musi być uruchomione.
- Użytkownik musi mieć dostęp do katalogu, w którym można utworzyć nowy plik.

**Kroki:**
1. Uruchomić edytor tekstowy "Cosmic".
2. Kliknąć na opcję "Plik" w górnym menu.
3. Wybrać opcję "Nowy".
4. Edytor powinien otworzyć pusty dokument.

**Oczekiwany wynik:**
- Powinien zostać utworzony pusty plik, a użytkownik powinien mieć możliwość wprowadzenia tekstu.
- Nazwa pliku powinna być tymczasowo "Bez tytułu" lub podobna.

**Scenariusz 2 (Użytkownik NIE ma uprawnień do zapisu w katalogu):**
- Po próbie zapisania pliku, system powinien wyświetlić komunikat o błędzie, informujący o braku uprawnień do zapisu w wybranym katalogu
- Plik nie powinien zostać zapisany, a katalog nie powinien zmienić swojego stanu.

---

## 4. TC-EDIT-04: Weryfikacja możliwości edycji zawartości pliku tekstowego
**Cel:** Sprawdzić, czy użytkownik może dodać lub usunąć tekst w otwartym pliku tekstowym.

**Warunki wstępne:**
- Oprogramowanie "Cosmic" musi być uruchomione.
- Użytkownik musi mieć otwarty plik tekstowy (np. `sample.txt`) w edytorze.

**Kroki:**
1. Uruchomić edytor tekstowy i otworzyć plik tekstowy.
2. Zmienić zawartość pliku poprzez dodanie nowego tekstu na końcu lub w dowolnym miejscu w pliku.
3. Usunąć istniejący tekst z pliku.

**Oczekiwany wynik:**
- Zmiany wprowadzone w tekście powinny być natychmiast widoczne w edytorze.
- Użytkownik powinien mieć możliwość dodawania i usuwania tekstu w pliku.

---

## 5. TC-EDIT-05: Weryfikacja możliwości zapisania zmian w edytowanym pliku tekstowym
**Cel:** Sprawdzić, czy użytkownik może zapisać zmiany dokonane w zawartości pliku tekstowego.

**Warunki wstępne:**
- Oprogramowanie "Cosmic" musi być uruchomione.
- Użytkownik musi mieć otwarty plik tekstowy, który był edytowany (np. zmieniono jego zawartość).

**Kroki:**
1. Uruchomić edytor tekstowy i otworzyć plik tekstowy, wprowadzić zmiany (np. dodanie lub usunięcie tekstu).
2. Kliknąć na opcję "Plik" w górnym menu.
3. Wybrać opcję "Zapisz" lub "Zapisz jako".
4. Jeżeli wybrano "Zapisz jako", wskazać odpowiednią lokalizację i kliknąć "Zapisz".

**Oczekiwany wynik:**
- Zmiany dokonane w pliku powinny zostać zapisane.
- Jeżeli plik został zapisany pod nową nazwą, to nowy plik powinien zawierać wprowadzone zmiany.

---

## 6. TC-EDIT-06: Weryfikacja możliwości zamknięcia edytora tekstu
**Cel:** Sprawdzić, czy użytkownik może zamknąć edytor tekstu, niezależnie od stanu otwartych lub edytowanych plików.

**Warunki wstępne:**
- Oprogramowanie "Cosmic" musi być uruchomione.
- Użytkownik może mieć otwarty plik tekstowy, w którym dokonano zmian, ale plik nie został zapisany.

**Kroki:**
1. Uruchomić edytor tekstowy "Cosmic" i otworzyć plik (opcjonalnie dokonać zmian).
2. Kliknąć na przycisk "X" w prawym górnym rogu okna aplikacji lub wybrać "Plik" -> "Zamknij".
3. Jeśli plik zawiera niezapisane zmiany, wybrać opcję, by zapisać plik lub odrzucić zmiany.

**Oczekiwany wynik:**
- Edytor powinien zamknąć się prawidłowo.
- Jeśli plik zawiera niezapisane zmiany, użytkownik powinien otrzymać komunikat z pytaniem, czy chce zapisać zmiany.
- Jeżeli użytkownik zdecyduje się nie zapisać, zmiany powinny zostać utracone.
