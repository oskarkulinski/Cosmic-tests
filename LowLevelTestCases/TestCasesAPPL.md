# Niskopoziomowe przypadki testowe dla COSMIC Applets

## LC-APPL-001

**Cel:** Sprawdzić, czy użytkownik jest informowany o fakcie podłączenia nowego urządzenia.

**Warunki wstępne:**

* Aktywna nakładka COSMIC
* Urządzenie, które będzie podłączane do komputera (w obrębie tego przypadku testowego przyjmujemy mysz komputerową z wyjściem USB, obsługująca wskaźnik pozycji x,y dla systemu wyświetlania)

**Kroki:**

1. Podłącz urządzenie do odpowiedniego interfejsu (wejścia).
2. Zweryfikuj, czy otrzymałeś komunikat o podłączeniu urządzenia.

**Oczekiwane wyniki:**

* Użytkownik jest informowany o podłączeniu urządzenia i wykrywany jest jego typ.

**Scenariusze pozytywne:**

1. **Podłączenie standardowego urządzenia USB:**
   * **Kroki:**
     1. Podłącz standardową mysz USB do komputera.
     2. Obserwuj powiadomienia na ekranie.
   * **Oczekiwane wyniki:**
     * System wyświetla komunikat informujący o podłączeniu myszy USB.
     * Typ urządzenia (mysz) jest poprawnie rozpoznany i wyświetlony.

2. **Podłączenie urządzenia z nowym sterownikiem:**
   * **Kroki:**
     1. Podłącz urządzenie USB, które wymaga instalacji nowego sterownika (np. zaawansowana mysz z dodatkowymi funkcjami).
     2. Obserwuj proces instalacji sterownika oraz powiadomienia.
   * **Oczekiwane wyniki:**
     * System informuje o potrzebie instalacji sterownika.
     * Po instalacji, komunikat potwierdza poprawne podłączenie urządzenia.

**Scenariusze negatywne:**

1. **Podłączenie uszkodzonego urządzenia USB:**
   * **Kroki:**
     1. Podłącz uszkodzoną mysz USB do komputera.
     2. Obserwuj powiadomienia na ekranie.
   * **Oczekiwane wyniki:**
     * System wyświetla komunikat o błędzie wykrywania urządzenia.
     * Użytkownik otrzymuje informację o problemie z urządzeniem.

2. **Podłączenie urządzenia niekompatybilnego z systemem:**
   * **Kroki:**
     1. Podłącz urządzenie USB, które nie jest wspierane przez system (np. specjalistyczny sprzęt).
     2. Obserwuj powiadomienia na ekranie.
   * **Oczekiwane wyniki:**
     * System wyświetla komunikat informujący o braku kompatybilności urządzenia.
     * Urządzenie nie jest rozpoznawane jako wspierane.

3. **Brak powiadomienia o podłączeniu urządzenia:**
   * **Kroki:**
     1. Podłącz mysz USB.
     2. Wyłącz powiadomienia systemowe.
     3. Obserwuj brak komunikatów na ekranie.
   * **Oczekiwane wyniki:**
     * System nie wyświetla żadnego komunikatu o podłączeniu urządzenia.
     * Użytkownik nie jest informowany o zmianie stanu urządzenia.

---

## LC-APPL-002

**Cel:** Sprawdzić, czy użytkownik może zobaczyć poziom naładowania baterii.

**Warunki wstępne:**

* Aktywna nakładka COSMIC
* Urządzenie, które posiada baterię (w obrębie tego przypadku testowego będzie to laptop)

**Kroki:**

1. Na górnym pasku zlokalizuj ikonę naładowania baterii.
2. Naciśnij na ikonę lub najedź kursorem.

**Oczekiwane wyniki:**

* Widoczny poziom naładowania baterii adekwatny do realnego poziomu naładowania.

**Scenariusze pozytywne:**

1. **Wyświetlenie poziomu baterii podczas normalnej pracy:**
   * **Kroki:**
     1. Upewnij się, że laptop jest uruchomiony i działa na baterii.
     2. Na górnym pasku nawigacyjnym znajdź ikonę baterii.
     3. Najedź kursorem na ikonę baterii.
   * **Oczekiwane wyniki:**
     * Pojawia się rozwijane okienko pokazujące dokładny procent naładowania baterii.
     * Dodatkowe informacje, takie jak pozostały czas pracy na baterii, są poprawnie wyświetlane.

2. **Aktualizacja poziomu baterii po zmianie stanu ładowania:**
   * **Kroki:**
     1. Podłącz laptop do źródła zasilania.
     2. Obserwuj ikonę baterii podczas ładowania.
     3. Odłącz laptop od źródła zasilania.
     4. Najedź kursorem na ikonę baterii.
   * **Oczekiwane wyniki:**
     * Ikona baterii pokazuje wzrost procentu podczas ładowania.
     * Po odłączeniu, ikona aktualizuje się, pokazując bieżący poziom naładowania.

**Scenariusze negatywne:**

1. **Brak aktualizacji poziomu baterii po odłączeniu zasilania:**
   * **Kroki:**
     1. Odłącz laptop od źródła zasilania.
     2. Najedź kursorem na ikonę baterii po kilku minutach.
   * **Oczekiwane wyniki:**
     * Ikona baterii nie aktualizuje się i pokazuje nieprawidłowy poziom naładowania.
     * System nie odzwierciedla rzeczywistego stanu baterii.

2. **Błędne wyświetlanie poziomu baterii:**
   * **Kroki:**
     1. Użyj laptopa na baterii i monitoruj poziom naładowania.
     2. Porównaj wyświetlany poziom z rzeczywistym zużyciem baterii.
   * **Oczekiwane wyniki:**
     * System pokazuje nieprawidłowy poziom naładowania, np. bateria jest rozładowana, ale system pokazuje 50%.

3. **Brak ikony baterii na pasku narzędzi:**
   * **Kroki:**
     1. Uruchom laptop na baterii.
     2. Sprawdź, czy ikona baterii jest widoczna na górnym pasku.
   * **Oczekiwane wyniki:**
     * Ikona baterii nie jest wyświetlana, co uniemożliwia użytkownikowi sprawdzenie poziomu naładowania.
     * Użytkownik nie ma dostępu do informacji o stanie baterii.

4. **Nieprawidłowe działanie interakcji z ikoną baterii:**
   * **Kroki:**
     1. Najedź kursorem na ikonę baterii.
     2. Kliknij na ikonę, aby wyświetlić szczegółowe informacje.
   * **Oczekiwane wyniki:**
     * System nie reaguje na interakcję, brak wyświetlenia szczegółowych informacji.
     * Użytkownik nie może uzyskać dodatkowych informacji o baterii.

---

## LC-APPL-003

**Cel:** Sprawdzić, czy każdy applet wyświetla te informacje, które powinien.

**Warunki wstępne:**

* Aktywna nakładka COSMIC

**Kroki:**

1. Na górnym pasku zlokalizować ikony:
    * Języka klawiatury (np. PL)
    * Głośności (głośnik)
    * Powiadomień (dymek wiadomości)
    * Wyłączania/resetowania urządzenia (klasyczny przycisk on/off)
    * Screen sharing/duplikacja ekranu (kilka prostokątów)
2. Sprawdzić, czy każda ikona po wejściu w interakcję (naciśnięciu ikony) pozwala na uzyskanie informacji dotyczących tego, co przedstawia.

**Oczekiwany wynik:**

* Możliwość:
    * Kontrolowania głośności
    * Zmiany języka klawiatury
    * Podejrzenia powiadomień
    * Wyłączenia/włączenia urządzenia
    * Udostępnienia/zduplikowania ekranu

    Po naciśnięciu odpowiadających funkcjonalnością ikon.

**Scenariusze pozytywne:**

1. **Poprawna interakcja z ikoną głośności:**
   * **Kroki:**
     1. Kliknij na ikonę głośności na górnym pasku.
     2. Zmień poziom głośności za pomocą suwaka.
   * **Oczekiwane wyniki:**
     * Suwak pozwala na płynne dostosowanie głośności.
     * Zmiany są natychmiast odzwierciedlane w systemie dźwiękowym.

2. **Zmiana języka klawiatury:**
   * **Kroki:**
     1. Kliknij na ikonę języka klawiatury (np. PL) na górnym pasku.
     2. Wybierz inny język, np. EN.
   * **Oczekiwane wyniki:**
     * Język klawiatury zmienia się na wybrany.
     * Ikona języka aktualizuje się, odzwierciedlając nowy wybór.

3. **Przeglądanie powiadomień:**
   * **Kroki:**
     1. Kliknij na ikonę powiadomień (dymek wiadomości) na górnym pasku.
     2. Przeglądaj listę otrzymanych powiadomień.
   * **Oczekiwane wyniki:**
     * Lista powiadomień jest poprawnie wyświetlana.
     * Użytkownik może czytać, usuwać lub odpowiadać na powiadomienia bez problemów.

4. **Wyłączanie urządzenia:**
   * **Kroki:**
     1. Kliknij na ikonę wyłączania/resetowania urządzenia (przycisk on/off).
     2. Wybierz opcję "Wyłącz" z menu.
   * **Oczekiwane wyniki:**
     * System rozpoczyna proces zamykania.
     * Urządzenie wyłącza się poprawnie po zakończeniu procesu.

5. **Udostępnianie ekranu:**
   * **Kroki:**
     1. Kliknij na ikonę screen sharing/duplikacji ekranu (kilka prostokątów) na górnym pasku.
     2. Wybierz opcję "Udostępnij ekran".
   * **Oczekiwane wyniki:**
     * Proces udostępniania ekranu rozpoczyna się bez błędów.
     * Użytkownik może wybrać, który ekran lub okno chce udostępnić.

**Scenariusze negatywne:**

1. **Nieprawidłowa reakcja ikony głośności:**
   * **Kroki:**
     1. Kliknij na ikonę głośności.
     2. Próbuj zmienić poziom głośności, ale suwak nie reaguje.
   * **Oczekiwane wyniki:**
     * Suwak głośności nie przesuwa się, a poziom dźwięku pozostaje niezmieniony.
     * System może wyświetlić komunikat o błędzie lub wymagać ponownego uruchomienia aplikacji.

2. **Błąd podczas zmiany języka klawiatury:**
   * **Kroki:**
     1. Kliknij na ikonę języka klawiatury.
     2. Wybierz nowy język.
   * **Oczekiwane wyniki:**
     * Język nie zmienia się, a ikona pozostaje w pierwotnym stanie.
     * System wyświetla komunikat o błędzie związanym ze zmianą języka.

3. **Brak wyświetlania powiadomień:**
   * **Kroki:**
     1. Kliknij na ikonę powiadomień.
     2. Sprawdź, czy lista powiadomień jest widoczna.
   * **Oczekiwane wyniki:**
     * Lista powiadomień nie jest wyświetlana mimo otrzymanych powiadomień.
     * Użytkownik nie może przeglądać ani zarządzać powiadomieniami.

4. **Nieudane wyłączanie urządzenia:**
   * **Kroki:**
     1. Kliknij na ikonę wyłączania urządzenia.
     2. Wybierz opcję "Wyłącz".
   * **Oczekiwane wyniki:**
     * System nie rozpoczyna procesu wyłączania.
     * Użytkownik otrzymuje komunikat o błędzie lub proces zamykania jest zawieszony.

5. **Problemy z udostępnianiem ekranu:**
   * **Kroki:**
     1. Kliknij na ikonę udostępniania ekranu.
     2. Wybierz opcję "Udostępnij ekran".
   * **Oczekiwane wyniki:**
     * Proces udostępniania nie rozpoczyna się, a użytkownik nie może wybrać ekranu do udostępnienia.
     * System wyświetla komunikat o błędzie związanym z udostępnianiem ekranu.

6. **Brak reakcji na kliknięcie ikony wyłączania:**
   * **Kroki:**
     1. Kliknij na ikonę wyłączania urządzenia.
     2. Naciśnij przycisk "Wyłącz" w menu.
   * **Oczekiwane wyniki:**
     * Przycisk nie reaguje na kliknięcie, a urządzenie nie rozpoczyna procesu wyłączania.
     * Użytkownik nie może zamknąć urządzenia poprzez interfejs appletu.

---
