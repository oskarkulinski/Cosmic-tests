# Rezultaty testów dla przypadków testowych niskopoziomowych Edytora Tekstowego "Cosmic"

## LC-EDIT-01  
**Rezultat**:  
Użytkownik może otworzyć dowolny plik tekstowy, jeśli posiada odpowiednie uprawnienia.  
**Test zaliczony dla scenariusza 1 (z uprawnieniami)**.

W przypadku braku uprawnień do odczytu pliku, edytor otworzył pusty dokument zamiast wyświetlić komunikat o błędzie.  
**Test niezaliczony dla scenariusza 2 (bez uprawnień)**.  

## LC-EDIT-02  
**Rezultat**:  
Użytkownik może zapisać otwarty plik tekstowy w dowolnym katalogu, do którego ma uprawnienia.  
W przypadku braku uprawnień do zapisu w katalogu, system poprawnie wyświetla komunikat o błędzie i plik nie zostaje zapisany.  
**Test zaliczony dla obu scenariuszy (z uprawnieniami i bez uprawnień)**.  

## LC-EDIT-03  
**Rezultat**:  
Użytkownik może utworzyć nowy, pusty plik tekstowy w edytorze.  
W przypadku próby zapisania pliku w katalogu bez odpowiednich uprawnień, wyświetlany jest komunikat o błędzie i plik nie zostaje zapisany.  
**Test zaliczony dla obu scenariuszy (z uprawnieniami i bez uprawnień)**.  

## LC-EDIT-04  
**Rezultat**:  
Użytkownik może edytować zawartość pliku tekstowego, dodając lub usuwając tekst. Zmiany są natychmiast widoczne w edytorze.  
**Test zaliczony, scenariusz 1 (sukces)**.  

## LC-EDIT-05  
**Rezultat**:  
Użytkownik może zapisać zmiany wprowadzone w pliku tekstowym. Zmiany są poprawnie odzwierciedlane w zapisanym pliku.  
**Test zaliczony, scenariusz 1 (sukces)**.  

## LC-EDIT-06  
**Rezultat**:  
Edytor tekstowy zamyka się prawidłowo.  
W przypadku niezapisanych zmian użytkownik otrzymuje komunikat z pytaniem, czy chce zapisać zmiany, co działa zgodnie z oczekiwaniami.  
**Test zaliczony, scenariusz 1 (sukces)**.
