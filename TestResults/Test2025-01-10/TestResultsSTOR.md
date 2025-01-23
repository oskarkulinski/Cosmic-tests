## Wyniki testów LC-STOR

### [LC-STOR-001](https://github.com/oskarkulinski/Cosmic-tests/blob/main/LowLevelTestCases/TestCasesSTOR.md#lc-stor-001)
- **Scenariusz:** Wyszukiwanie pełną nazwą.  
  **Rezultat:** Po wpisaniu pełnej nazwy aplikacji w pole wyszukiwania aplikacja zostaje poprawnie odnaleziona.  
  **Test zaliczony.**

- **Scenariusz:** Wyszukiwanie częściową nazwą.  
  **Rezultat:** Po wpisaniu niepełnej nazwy aplikacji w pole wyszukiwania aplikacja zostanie poprawnie odnaleziona.  
  **Test zaliczony.**

- **Scenariusz:** Wyszukiwanie nieistniejącej aplikacji.  
  **Rezultat:** Po wpisaniu nazwy nieistniejącej aplikacji w pole wyszukiwania lista wyników jest pusta i wyświetla się odpowiedni komunikat.  
  **Test zaliczony.**

- **Scenariusz:** Wyszukiwanie z użyciem znaków specjalnych.  
  **Rezultat:** Po wpisaniu nazwy aplikacji ze znakami specjalnymi w pole wyszukiwania lista wyników jest pusta i wyświetla się odpowiedni komunikat.  
  **Test zaliczony.**

---

### [LC-STOR-002](https://github.com/oskarkulinski/Cosmic-tests/blob/main/LowLevelTestCases/TestCasesSTOR.md#lc-stor-002)
- **Scenariusz:** Kliknięcie przycisku instalacji.  
  **Rezultat:** Po kliknięciu przycisku rozpoczyna się proces instalacji.  
  **Test zaliczony.**

- **Scenariusz:** Instalacja przy stabilnym połączeniu internetowym.  
  **Rezultat:** Instalacja przebiega bez przerw i kończy się sukcesem.  
  **Test zaliczony.**

- **Scenariusz:** Brak przycisku instalacji dla już zainstalowanej aplikacji.  
  **Rezultat:** Brak przycisku 'Zainstaluj', co uniemożliwia ponowną instalację aplikacji.  
  **Test zaliczony.**

- **Scenariusz:** Kliknięcie przycisku instalacji bez aktywnego połączenia internetowego.  
  **Rezultat:** Po kliknięciu 'Zainstaluj' pojawia się komunikat o braku aktywnego połączenia internetowego.  
  **Test zaliczony.**

- **Scenariusz:** Przycisk instalacji jest nieaktywny.  
  **Rezultat:** Brak.  
  **Test nieprzeprowadzony** ze względu na brak możliwości dezaktywacji przycisku.

---

### [LC-STOR-003](https://github.com/oskarkulinski/Cosmic-tests/blob/main/LowLevelTestCases/TestCasesSTOR.md#lc-stor-003)
- **Scenariusz:** Instalacja i uruchomienie aplikacji bez błędów.  
  **Rezultat:** Aplikacja zostaje zainstalowana, sklep aktualizuje status instalacji aplikacji.  
  **Test zaliczony.**

- **Scenariusz:** Instalacja na systemie z ograniczonym miejscem na dysku.  
  **Rezultat:** Aplikacja instaluje się poprawnie, sklep aktualizuje status instalacji.  
  **Test zaliczony.**

- **Scenariusz:** Błędna instalacja aplikacji.  
  **Rezultat:** Brak.  
  **Test nieprzeprowadzony** ze względu na brak możliwości przerwania procesu instalacji.

- **Scenariusz:** Niewystarczające uprawnienia do instalacji.  
  **Rezultat:** Użytkownik mimo braku uprawnień jest w stanie zainstalować aplikację.  
  **Test niezaliczony.**

---

### [LC-STOR-004](https://github.com/oskarkulinski/Cosmic-tests/blob/main/LowLevelTestCases/TestCasesSTOR.md#lc-stor-004)
- **Scenariusz:** Odinstalowanie aplikacji poprzez sklep.  
  **Rezultat:** Aplikacja zostaje odinstalowana.  
  **Test zaliczony.**

- **Scenariusz:** Odinstalowanie aplikacji i ponowna instalacja.  
  **Rezultat:** Aplikacja została odinstalowana, a ponowna instalacja przechodzi bez problemów.  
  **Test zaliczony.**

- **Scenariusz:** Odinstalowanie aplikacji bez uprawnień.  
  **Rezultat:** Użytkownik mimo braku uprawnień może odinstalować aplikację.  
  **Test niezaliczony.**

- **Scenariusz:** Przerwanie procesu odinstalowania.  
  **Rezultat:** Brak.  
  **Test nieprzeprowadzony** ze względu na brak możliwości przerwania odinstalowania aplikacji.

- **Scenariusz:** Odinstalowanie aplikacji, która nie jest zainstalowana.  
  **Rezultat:** Brak możliwości odinstalowania aplikacji, która nie jest zainstalowana.  
  **Test zaliczony.**

---

### [LC-STOR-005](https://github.com/oskarkulinski/Cosmic-tests/blob/main/LowLevelTestCases/TestCasesSTOR.md#lc-stor-005)
- **Scenariusz:** Pełne usunięcie aplikacji z systemu.  
  **Rezultat:** Aplikacja została w pełni usunięta z systemu.  
  **Test zaliczony.**

- **Scenariusz:** Odinstalowanie aplikacji i sprawdzenie czystości systemu.  
  **Rezultat:** System jest wolny od wszystkich plików i wpisów związanych z aplikacją.  
  **Test zaliczony.**

- **Scenariusz:** Usunięcie aplikacji, podczas gdy są otwarte pliki.  
  **Rezultat:** System nie pozwala na odinstalowanie aplikacji, gdy są otwarte edytowane pliki.  
  **Test zaliczony.**

- **Scenariusz:** Niepełne usunięcie aplikacji.  
  **Rezultat:** Wszystkie elementy aplikacji zostały usunięte prawidłowo, brak problemów.  
  **Test zaliczony.**

- **Scenariusz:** Błąd podczas odinstalowania.  
  **Rezultat:** Brak miejsca na dysku nie wpływa na możliwość odinstalowania aplikacji.  
  **Test niejednoznaczny.**
