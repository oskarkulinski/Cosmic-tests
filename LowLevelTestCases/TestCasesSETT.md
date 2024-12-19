# Przypadki testowe dla COSMIC settings.

## LC-SETT-001 Weryfikacja możliwości zmiany ustawień.   
**Cel**: Sprawdzić, czy użytkownik może zmieniać ustawienia.
**Warunki wstępne**
- Otworzony edytor ustawień COSMIC

**Kroki**
1. Zmienić ustawienie, o ile interfejs graficzny sugeruje taką możliwośc, zależnie od typu, dla:
    - ustawień o zakresie wykonać test dla maksymalnej, minimalnej, oraz środkowej wartości.
    - ustawień z listą wyborów, przetestować dla wybór pierwszej, drugiej, i ostatniej pozycji z listy, lub wszystkich jej pozycji jeśli jest ich mniej niż 3, nie dotyczy to ustawienia łączenia się z WIFI.
    - ustawień typu przełącznik/checkbox, przetestować zaznaczanie i odznaczanie.
    - dla zmiany tapety, wybrać dowolny obraz pobrany z internetu.
    - dla pozostałych ustawień nie wykonujemy testów, ze względu na trudność ich przetestowania.

**Oczekiwane wyniki**   
- **Scenariusze pozytywne**   
    1. Ustawienie zostało zmienione.
    **Scenariusze negatywne**
    2. Ustawienia nie można zmienić.

## LC-SETT-002

Weryfikacja możliwości zapisu zmienionych ustawień.   
**Cel**: Sprawdzić, czy użytkownik może zapisać zmienione ustawienia.
**Warunki wstępne**
- Otworzony edytor ustawień COSMIC

**Kroki**
1. Zmienić ustawienie, o ile interfejs graficzny sugeruje taką możliwośc, zależnie od typu, dla:
    - ustawień o zakresie wykonać test dla maksymalnej, minimalnej, oraz środkowej wartości.
    - ustawień z listą wyborów, przetestować dla wybór pierwszej, drugiej, i ostatniej pozycji z listy, lub wszystkich jej pozycji jeśli jest ich mniej niż 3, nie dotyczy to ustawienia łączenia się z WIFI.
    - ustawień typu przełącznik/checkbox, przetestować zaznaczanie i odznaczanie.
    - dla zmiany tapety, wybrać dowolny obraz pobrany z internetu.
    - dla pozostałych ustawień nie wykonujemy testów, ze względu na trudność ich przetestowania.
2. Zamknąć edytor ustawień COSMIC.
3. Otworzyć edytor ustawień COSMIC.
4. Zweryfikować czy ustawienie zostało zapisane.

**Oczekiwane wyniki**   
- **Scenariusze pozytywne**   
    1. Ustawienie zostało zapisane.
    **Scenariusze negatywne**
    2. Ustawienie nie zostało zapisane.
    3. Ustawienie zostało zapisane, ale błędnie. Na przykład, zmieniono ustawienie ze stanu A na stan B a po restarcie aplikacji ustawienie jest w stanie C.


## LC-SETT-003

Weryfikacja możliwości doświadczenia wpływu zmiany ustawień na stan systemu operacyjnego.   
**Cel**: Sprawdzić, czy po zmianie i zapisaniu ustawień mają one realny wpływ na system operacyjny, zgodny ze swoim opisem, lub intuicją użytkownika.
**Warunki wstępne**
- Otworzony edytor ustawień COSMIC

**Kroki**
1. Zmienić ustawienie, o ile interfejs graficzny sugeruje taką możliwośc, zależnie od typu, dla:
    - ustawień o zakresie wykonać test dla maksymalnej, minimalnej, oraz środkowej wartości.
    - ustawień z listą wyborów, przetestować dla wybór pierwszej, drugiej, i ostatniej pozycji z listy, lub wszystkich jej pozycji jeśli jest ich mniej niż 3, nie dotyczy to ustawienia łączenia się z WIFI.
    - ustawień typu przełącznik/checkbox, przetestować zaznaczanie i odznaczanie.
    - dla zmiany tapety, wybrać dowolny obraz pobrany z internetu.
    - dla pozostałych ustawień nie wykonujemy testów, ze względu na trudność ich przetestowania.
2. Zweryfikować czy zmiana ustawienia wpłynęła na system operacyjny w sposób zgodny z nazwą, opisem i intuicją użytkownika.

**Oczekiwane wyniki**   
- **Scenariusze pozytywne**   
    1. Ustawienie wpłynęło na system zgodnie z oczekiwaniem.
    **Scenariusze negatywne**
    2. Ustawienie nie wpłynęło na system.
    3. Ustawienie wpłynęło na system, ale w sposób niezgodny z oczekiwaniem, na przykład po zmianie głośności ta pozostała nie zmieniona a zmieniła się jasność ekranu.


