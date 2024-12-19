# Niskopoziomowe przypadki testowe dla COSMIC Store

## LC-STOR-001

**Cel:** Sprawdzić czy po wpisaniu nazwy aplikacji w pole wyszukiwania, aplikacja zostanie poprawnie odnaleziona.

**Warunki wstępne:**

* Aktywna nakładka COSMIC
* Wybrana aplikacja, która jest dostępna w sklepie posiadanej dystrybucji (w obrębie tego przypadku testowego przyjmijmy, że jest to Visual Studio Code)
* Włączona aplikacja sklepu

**Kroki:**

1. W pole do wyszukiwania wpisać konkretną nazwę szukanej aplikacji (tutaj Visual Studio Code), która jest dostępna w sklepie POP_OS (lub innej dystrybucji systemu Linux).

**Oczekiwane wyniki:**

* Aplikacja (tutaj Visual Studio Code) wyświetla się w liście wyszukiwań, możemy odwiedzić stronę sklepu tej aplikacji.

**Scenariusze pozytywne:**

1. **Wyszukiwanie pełną nazwą:**
   * **Kroki:**
     1. Wpisz pełną nazwę aplikacji "Visual Studio Code" w pole wyszukiwania.
   * **Oczekiwane wyniki:**
     * Aplikacja zostaje natychmiast odnaleziona i wyświetlona na górze listy wyników.

2. **Wyszukiwanie częściową nazwą:**
   * **Kroki:**
     1. Wpisz część nazwy aplikacji, np. "Visual" lub "Code".
   * **Oczekiwane wyniki:**
     * Aplikacje zawierające wpisany fragment w nazwie, w tym Visual Studio Code, są wyświetlane w wynikach wyszukiwania.

**Scenariusze negatywne:**

1. **Wyszukiwanie nieistniejącej aplikacji:**
   * **Kroki:**
     1. Wpisz losową, nieistniejącą nazwę aplikacji, np. "AppXYZ123" w pole wyszukiwania.
   * **Oczekiwane wyniki:**
     * Lista wyników jest pusta lub wyświetla komunikat o braku znalezionych aplikacji.

2. **Wyszukiwanie z użyciem znaków specjalnych:**
   * **Kroki:**
     1. Wpisz nazwę z nieprawidłowymi znakami, np. "Visual@#Code".
   * **Oczekiwane wyniki:**
     * System ignoruje znaki specjalne i próbuje znaleźć aplikację na podstawie poprawnych części nazwy lub wyświetla komunikat o błędzie.

---

## LC-STOR-002

**Cel:** Sprawdzić, czy po wybraniu aplikacji możemy ją zainstalować na urządzeniu, i czy zostanie przeprowadzony proces instalacji.

**Warunki wstępne:**

* Aktywna nakładka COSMIC
* Wybrana aplikacja, która jest dostępna w sklepie posiadanej dystrybucji (w obrębie tego przypadku testowego przyjmijmy, że jest to Visual Studio Code)
* Włączona aplikacja sklepu i aktywna strona sklepu dla aplikacji (tutaj Visual Studio Code)

**Kroki:**

1. Znajdź na stronie sklepu aplikacji przycisk odpowiadający za rozpoczęcie instalacji.

**Oczekiwane wyniki:**

* Na stronie sklepu aplikacji znajduje się przycisk umożliwiający zainstalowanie.

**Scenariusze pozytywne:**

1. **Kliknięcie przycisku instalacji:**
   * **Kroki:**
     1. Kliknij przycisk "Zainstaluj" na stronie Visual Studio Code w sklepie.
   * **Oczekiwane wyniki:**
     * Proces instalacji rozpoczyna się, a użytkownik widzi postęp instalacji.

2. **Instalacja przy stabilnym połączeniu internetowym:**
   * **Kroki:**
     1. Upewnij się, że połączenie internetowe jest stabilne, a następnie kliknij "Zainstaluj".
   * **Oczekiwane wyniki:**
     * Instalacja przebiega bez przerw i kończy się sukcesem.

**Scenariusze negatywne:**

1. **Brak przycisku instalacji dla już zainstalowanej aplikacji:**
   * **Kroki:**
     1. Próbuj zainstalować aplikację, która jest już zainstalowana.
   * **Oczekiwane wyniki:**
     * Przycisk "Zainstaluj" jest zastąpiony przez "Otwórz" lub "Zaktualizuj", uniemożliwiając ponowną instalację.

2. **Kliknięcie przycisku instalacji bez aktywnego połączenia internetowego:**
   * **Kroki:**
     1. Wyłącz połączenie internetowe i kliknij "Zainstaluj".
   * **Oczekiwane wyniki:**
     * Wyświetla się komunikat o błędzie związanym z brakiem połączenia internetowego, a instalacja nie rozpoczyna się.

3. **Przycisk instalacji jest nieaktywny:**
   * **Kroki:**
     1. Kliknij przycisk instalacji, który jest widoczny, ale nie reaguje na kliknięcie.
   * **Oczekiwane wyniki:**
     * Aplikacja reaguje odpowiednim komunikatem błędu lub przycisk zostaje odblokowany.

---

## LC-STOR-003

**Cel:** Sprawdzić, czy aplikacja po zakończeniu instalacji znajduje się na dysku systemu operacyjnego, jest dostępna i funkcjonalna, oraz czy informacja o tym jest wyświetlana w sklepie.

**Warunki wstępne:**

* Aktywna nakładka COSMIC
* Wybrana aplikacja, która jest dostępna w sklepie posiadanej dystrybucji (w obrębie tego przypadku testowego przyjmijmy, że jest to Visual Studio Code), która została wcześniej zainstalowana (jak w przypadku TC-STOR-002)
* Włączona aplikacja sklepu i aktywna strona sklepu dla aplikacji (tutaj Visual Studio Code)

**Kroki:**

1. Naciśnij przycisk odpowiadający za rozpoczęcie instalacji.
2. Poczekaj, aż instalacja się zakończy.
3. Jeśli instalacja nie kończy się zweryfikuj swoje połączenie z internetem.
4. Zweryfikuj, czy w miejscu gdzie domyślnie instalowane są aplikacje ze sklepu znajdują się pliki wybranej aplikacji (tutaj Visual Studio Code).
5. Włącz aplikację.
6. Spróbuj wykonać czynności typowe dla aplikacji (w tym przypadku edycja pliku tekstowego i jego zapisanie).
7. Sprawdź, czy w sklepie widać, że aplikacji nie możemy już zainstalować tylko ją usunąć.

**Oczekiwane wyniki:**

* Można rozpocząć proces instalacji
* Instalacja kończy się
* Pliki aplikacji znajdują się na dysku tam, gdzie powinny
* Aplikacja włącza się
* Aplikacja jest funkcjonalna (możemy wykonywać typowe dla niej czynności)
* Sklep pokazuje, że stan instalacji aplikacji jest adekwatny do tego, co jest na dysku

**Scenariusze pozytywne:**

1. **Instalacja i uruchomienie aplikacji bez błędów:**
   * **Kroki:**
     1. Przeprowadź instalację Visual Studio Code zgodnie z powyższymi krokami.
   * **Oczekiwane wyniki:**
     * Aplikacja instaluje się bez problemów, pliki są poprawnie umieszczone, aplikacja działa bez błędów, a sklep prawidłowo aktualizuje status instalacji.

2. **Instalacja na systemie z ograniczonym miejscem na dysku:**
   * **Kroki:**
     1. Upewnij się, że na dysku jest minimalna ilość wolnego miejsca potrzebna do instalacji i przeprowadź instalację.
   * **Oczekiwane wyniki:**
     * Aplikacja instaluje się poprawnie, a sklep aktualizuje status instalacji, informując użytkownika o dostępnej przestrzeni.

**Scenariusze negatywne:**

1. **Błędna instalacja aplikacji:**
   * **Kroki:**
     1. Przerwij proces instalacji w trakcie jego trwania.
   * **Oczekiwane wyniki:**
     * Instalacja się nie kończy, sklep wyświetla komunikat o błędzie, a na dysku nie pojawiają się pliki aplikacji.

2. **Niewystarczające uprawnienia do instalacji:**
   * **Kroki:**
     1. Próbuj zainstalować aplikację bez odpowiednich uprawnień (np. jako użytkownik bez praw administratora).
   * **Oczekiwane wyniki:**
     * Instalacja się nie rozpoczyna lub wyświetla komunikat o braku uprawnień, a aplikacja nie jest instalowana.

---

## LC-STOR-004

**Cel:** Weryfikacja poprawnej możliwości odinstalowania aplikacji w sklepie.

**Warunki wstępne:**

* Aktywna nakładka COSMIC
* Wybrana aplikacja, która jest dostępna w sklepie posiadanej dystrybucji (w obrębie tego przypadku testowego przyjmijmy, że jest to Visual Studio Code), która została wcześniej zainstalowana (jak w przypadku TC-STOR-003)
* Włączona aplikacja sklepu i aktywna strona sklepu dla aplikacji (tutaj Visual Studio Code)

**Kroki:**

1. Znajdź na stronie sklepu tej aplikacji (tutaj Visual Studio Code) przycisk odpowiadający za odinstalowanie.

**Oczekiwane wyniki:**

* Na stronie sklepu tej aplikacji widać przycisk umożliwiający odinstalowanie

**Scenariusze pozytywne:**

1. **Odinstalowanie aplikacji poprzez sklep:**
   * **Kroki:**
     1. Kliknij przycisk "Odinstaluj" na stronie Visual Studio Code w sklepie.
   * **Oczekiwane wyniki:**
     * Proces odinstalowania rozpoczyna się, a użytkownik otrzymuje potwierdzenie zakończenia odinstalowania.

2. **Odinstalowanie aplikacji i ponowna instalacja:**
   * **Kroki:**
     1. Odinstaluj aplikację Visual Studio Code, a następnie ponownie zainstaluj ją poprzez sklep.
   * **Oczekiwane wyniki:**
     * Aplikacja zostaje poprawnie odinstalowana, a następnie ponownie zainstalowana bez błędów.

**Scenariusze negatywne:**

1. **Odinstalowanie aplikacji bez uprawnień:**
   * **Kroki:**
     1. Próbuj odinstalować aplikację bez odpowiednich uprawnień (np. jako użytkownik bez praw administratora).
   * **Oczekiwane wyniki:**
     * Proces odinstalowania się nie rozpoczyna lub wyświetla komunikat o braku uprawnień.

2. **Przerwanie procesu odinstalowania:**
   * **Kroki:**
     1. Rozpocznij proces odinstalowania i przerwij go przed zakończeniem (np. zamykając sklep).
   * **Oczekiwane wyniki:**
     * Proces odinstalowania się nie kończy poprawnie, a aplikacja pozostaje częściowo odinstalowana lub w stanie niepełnej funkcjonalności.

3. **Odinstalowanie aplikacji, która nie jest zainstalowana:**
   * **Kroki:**
     1. Próbuj odinstalować aplikację, która nie została wcześniej zainstalowana.
   * **Oczekiwane wyniki:**
     * Sklep wyświetla komunikat, że aplikacja nie jest zainstalowana, uniemożliwiając odinstalowanie.

---

## LC-STOR-005

**Cel:** Sprawdzić, czy po odinstalowaniu aplikacja jest poprawnie usuwana z systemu operacyjnego i czy

**Warunki wstępne:**

* Aktywna nakładka COSMIC
* Wybrana aplikacja, która jest dostępna w sklepie posiadanej dystrybucji (w obrębie tego przypadku testowego przyjmijmy, że jest to Visual Studio Code), która została wcześniej zainstalowana (jak w przypadku TC-STOR-003)
* Włączona aplikacja sklepu i aktywna strona sklepu dla aplikacji (tutaj Visual Studio Code)
* Otwarte katalogi, w których znajdują się pliki związane z naszą aplikacją

**Kroki:**

1. Naciśnij przycisk służący do odinstalowania aplikacji.
2. Poczekaj aż proces odinstalowania się zakończy.
3. Zweryfikuj, czy w miejscu gdzie wcześniej znajdowały się pliki aplikacji teraz ich nie ma.
4. Sprawdź, czy w sklepie widnieje ponowna możliwość zainstalowania aplikacji.

**Oczekiwane wyniki:**

* Można rozpocząć proces odinstalowania
* Proces odinstalowania się kończy
* Aplikacja jest poprawnie usuwana z dysku systemu operacyjnego
* W sklepie możemy ponownie zainstalować aplikację

**Scenariusze pozytywne:**

1. **Pełne usunięcie aplikacji z systemu:**
   * **Kroki:**
     1. Przeprowadź proces odinstalowania Visual Studio Code zgodnie z powyższymi krokami.
   * **Oczekiwane wyniki:**
     * Wszystkie pliki aplikacji są usunięte z dysku, aplikacja jest wyłączona, a sklep umożliwia jej ponowną instalację.

2. **Odinstalowanie aplikacji i sprawdzenie czystości systemu:**
   * **Kroki:**
     1. Odinstaluj Visual Studio Code, a następnie przeprowadź skanowanie systemu w poszukiwaniu pozostałości plików.
   * **Oczekiwane wyniki:**
     * Nie ma żadnych pozostałości plików ani wpisów rejestru związanych z aplikacją.

**Scenariusze negatywne:**

1. **Usunięcie aplikacji, podczas gdy są otwarte pliki:**
   * **Kroki:**
     1. Odinstaluj Visual Studio Code, podczas gdy otwarte są edytowane pliki w aplikacji.
   * **Oczekiwane wyniki:**
     * System wyświetla ostrzeżenie o otwartych plikach, a proces odinstalowania wymaga zamknięcia aplikacji przed kontynuacją.

2. **Niepełne usunięcie aplikacji:**
   * **Kroki:**
     1. Przeprowadź proces odinstalowania Visual Studio Code i sprawdź, czy wszystkie pliki zostały usunięte.
   * **Oczekiwane wyniki:**
     * Niektóre pliki lub foldery pozostają na dysku, co może wskazywać na problem z procesem odinstalowania.

3. **Błąd podczas odinstalowania:**
   * **Kroki:**
     1. Spróbuj odinstalować aplikację, gdy system operacyjny napotyka na błąd (np. brak miejsca na dysku).
   * **Oczekiwane wyniki:**
     * Proces odinstalowania się nie kończy poprawnie, a użytkownik otrzymuje komunikat o błędzie, a aplikacja nie jest w pełni usunięta.

---
