# LC-COMP-001: Weryfikacja działania zmiennej częstotliwości odświeżania ekranu, dla jednego monitora.
**Cel:** Sprawdzić, czy zmienna częstotliwość odświeżania ekranu działa przy podłączonym jednym monitorze.   
**Warunki wstępne:**
- Zainstalowany VRRTest - https://github.com/Nixola/VRRTest   
**Kroki:**
1. Uruchomić VRRTest.
2. Zmniejszyc ilość klatek na sekundę, poniżej poziomu częstotliwości odświeżania ekranu.

**Oczekiwane wyniki:**
- Niezależnie od ilości klatek na sekundę paski przesuwają się po ekranie płynnie, bez zacięć i przeskoków.
**Scenariusze pozytywne**
1. Zmienna częstotliwość odświeżania działa.   
    - Kroki:   
        - Sprawdź czy niezależnie od ilości klatek na sekundę paski przesuwają się po ekranie płynnie, bez zacięć i przeskoków.  
    - Oczekiwane wyniki:   
        -  Niezależnie od ilości klatek na sekundę paski przesuwają się po ekranie płynnie, bez zacięć i przeskoków.

**Scenariusze negatywne**
1. Zmienna częstotliwość odświeżania działa.   
    - Kroki:   
        - Sprawdź czy niezależnie od ilości klatek na sekundę paski przesuwają się po ekranie płynnie, bez zacięć i przeskoków.  
    - Oczekiwane wyniki:   
        -  Paski zacinają się lub przeskakują, brakuje płynności.

# LC-COMP-002: Weryfikacja działania zmiennej częstotliwości odświeżania ekranu, dla dwóch monitorów.
**Cel:** Sprawdzić, czy zmienna częstotliwość odświeżania ekranu działa przy podłączonych dwóch monitorach.   
**Warunki wstępne:**
- Zainstalowany VRRTest - https://github.com/Nixola/VRRTest
- Monitor z funkcją zmiennej częstotliwości odświeżania ekranu.   
**Kroki:**
1. Uruchomić VRRTest na głownym monitorze.
2. Zmniejszyc ilość klatek na sekundę, poniżej poziomu częstotliwości odświeżania ekranu.
**Oczekiwane wyniki:**
- Niezależnie od ilości klatek na sekundę paski przesuwają się po ekranie płynnie, bez zacięć i przeskoków.
**Scenariusze pozytywne**
1. Zmienna częstotliwość odświeżania działa.   
    - Kroki:   
        - Sprawdź czy niezależnie od ilości klatek na sekundę paski przesuwają się po ekranie płynnie, bez zacięć i przeskoków.  
    - Oczekiwane wyniki:   
        -  Niezależnie od ilości klatek na sekundę paski przesuwają się po ekranie płynnie, bez zacięć i przeskoków.

**Scenariusze negatywne**
1. Zmienna częstotliwość odświeżania działa.   
    - Kroki:   
        - Sprawdź czy niezależnie od ilości klatek na sekundę paski przesuwają się po ekranie płynnie, bez zacięć i przeskoków.  
    - Oczekiwane wyniki:   
        -  Paski zacinają się lub przeskakują, brakuje płynności.
