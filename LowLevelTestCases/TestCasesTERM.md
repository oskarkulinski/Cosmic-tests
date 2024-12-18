# Niskopoziomowe Przypadki Testowe dla Terminala

## 1. TC-TERM-001

**Cel:** Zweryfikować, czy użytkownik jest w stanie poprawnie wprowadzić dowolną komendę obsługiwaną przez interpretera Bash.

**Warunki wstępne:**
- Użytkownik musi mieć uprawnienia do uruchamiania terminala..

**Kroki:**
1. Uruchomić terminal.
2. Wprowadzić dowolną komendę obsługiwaną przez Bash.
3. Nacisnąć Enter.

**Oczekiwany wynik:**
- W przypadku poprawnej komendy terminal wyświetli odpowiednią odpowiedź.
- W przypadku niepoprawnej komendy terminal wyświetli komunikat o błędzie.


## 2. TC-TERM-002

**Cel:** Zweryfikować, czy użytkownik może przeglądać historię wpisanych komend w terminalu za pomocą klawisza **strzałka w górę**.

**Warunki wstępne:**
- Użytkownik musi mieć uprawnienia do uruchamiania terminala.
- W historii terminala muszą znajdować się wcześniej wpisane komendy.

**Kroki:**
1. Uruchomić terminal.
2. Wprowadzić kilka różnych oraz poprawnych komend i nacisnąć Enter po każdej z nich.
3. Nacisnąć klawisz **strzałka w górę**.

**Oczekiwany wynik:**
- Terminal wyświetli poprzednio wpisane komendy w odwrotnej kolejności.
- Użytkownik będzie mógł edytować wybraną komendę przed jej ponownym uruchomieniem.

**Scenariusz alternatywny (Historia jest pusta):**
- Naciśnięcie klawisza **strzałka w górę** nie spowoduje żadnej zmiany w terminalu, ponieważ historia komend jest pusta.
