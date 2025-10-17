# Merge Konflikt Analys


##Felet som uppstod:
    "Auto-merging index.html
    CONFLICT (content): Merge conflict in index.html
    Automatic merge failed; fix conflicts and then commit the result."
    
## Orsak
    Konflikten uppstod eftersom både feature/alpha och feature/beta ändrade samma rad (<h1>taggen) vilket gjorde att Git inte kunde avgöra vilken version som skulle behållas.

## Lösning  
Konflikten löstes genom att manuellt välja vilken version som skulle behållas i VS Code:s merge conflict editor, där vi valde (Accept Current/Incoming), tog bort konfliktmarkörerna (<<<<<<, =======, >>>>>>) och valde den slutgiltiga versionen av koden.

## Förebyggande
För att undvika sådana konflikter i framtiden bör man kommunicera om vilka filer som ändras samt merga main-branchen till feature-brancher för att hålla dem uppdaterade.
