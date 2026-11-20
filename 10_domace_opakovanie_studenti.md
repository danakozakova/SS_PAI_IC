# Otvorené otázky na opakovanie

Odpovedz vlastnými slovami. Pri otázkach s kódom napíš, čo sa stane a prečo.

## A. Zápis a typy
1. Ako sa v Pythone zapisuje **n-tica (tuple)**? Ako sa zapisuje **zoznam**, **slovník** a **množina**?
2. Ako vytvoríš **prázdny slovník** a ako **prázdnu množinu**? Čo vznikne zápisom `x = {}`?
3. Ktoré dátové typy sú **immutable (nemeniteľné)** a ktoré **mutable (meniteľné)**?
4. Akou funkciou zistíš **typ** hodnoty? Čo vráti `type("5")` a čo `type(5)`?
5. Ako sa v Pythone správne zapíše desatinné číslo? (Pozor na rozdiel oproti bežnému písaniu v slovenčine.)

## B. Konverzie
6. V ktorých z týchto príkladov nastáva **automatická konverzia** typu a aký bude výsledok?
   ```python
   3 / 2
   True + True
   3 + 2.5
   "5" + 5
   ```
   Pri ktorom nastane **chyba** a prečo?
7. Prečo `vek = input("...")` vráti vždy `str`? Čo musíš urobiť, ak chceš s hodnotou počítať?
8. Ktoré prevody prebehnú bez chyby a ktoré spadnú: `int("12")`, `int("12.5")`, `int("abc")`, `float("3.5")`? Prečo?

## C. Metódy, meniteľnosť, priradenie
9. Prečo pri `zoznam.sort()` **nepoužívame** priradenie (`zoznam = zoznam.sort()`), ale pri `veta.strip()` priradenie **potrebujeme**?
10. Aký je rozdiel medzi **metódou** (`objekt.metoda()`) a **všeobecnou funkciou** ako `len()`?
11. Čo sa stane po `t = (1, 2, 3)` a potom `t.sort()`? Prečo?
12. Čo bude vo `vysledok` po `veta = "  AhOj  "` a `vysledok = veta.strip().upper()`?

## D. Výber správneho typu
13. Aký dátový typ použiješ pre: zoznam známok, ktorý sa mení · nemenné súradnice `(49, 19)` · osobné údaje (meno, vek, email) · zoznam unikátnych navštívených krajín? Zdôvodni.
14. Prečo je bezpečnejšie `student.get("email", "neuvedený")` než `student["email"]`?

## E. Množiny
15. Aký je hlavný rozdiel medzi **zoznamom** a **množinou**?
16. Čo vráti `{1, 2, 3} & {2, 3, 4}` a čo `{1, 2, 3} | {2, 3, 4}`?
