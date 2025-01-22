# Škrábance ledu

<details>
<summary>Krok 1. Škrábance</summary>
Škrábance vytvoříme pomocí uzlu **Textura Voronoi**. Přidejte ji a upravte následovně:
- **Typ** uzlu změňte z F1 na **Distance to edge**
- **Velikost** na 0.8

Tento uzel také připojte za **Mapování** a následně přidejte za Texturu Voronoi uzel **Rampa barev** kde nejdříve posuvník s černou barvou posuňte úplně doleva, a následně tam posuňte i druhý s bílou barvou. Měli byste dosáhnou úzkých linek.
![L7](https://github.com/user-attachments/assets/a1552d82-abb2-4eb4-a2ba-e42eaab81ddf)

</details>
<details>
<summary>Krok 2. Maska pro výskyt škrábanců</summary>
Masku, kterou omezíme výskyt škrábanců založíme na uzlu **Textura šumu**. Vložte jej a nastavte takto:
- **Velikost** na 2
- **Detail** na maximum

Dále za tento uzel připojte novou **Rampu barev**, kde hodnoty bílé a černé dejte velmi blízko sobě pro zvýraznění kontrastu.
![L8](https://github.com/user-attachments/assets/cd3cbbb3-1782-4f8c-ba4c-12e16f484862)

</details>
<details>
<summary>Krok 3. Aplikace masky</summary>
 
Maskou vyhraničíme oblasti kde se mají škrábance projevovat připojíme pomocí uzlu **Mix color**. Přidejte jej do prostředí a do vstupu Faktor připojte výstup z Rampy barev od masky, a do barvy A připojte Rampu barev ze škrábancové skupiny.
![L9](https://github.com/user-attachments/assets/78791ba7-69eb-40f1-8337-5f8086931820)

</details>
<details>

<summary>Krok 4. Připojení do normálových dat</summary>

Konečně škrábance připojíme do normálové mapy a to znovu s uzlem **Bump**. Duplikujte uzel z minulé kapitoly a výstup nového připojte do normálového vstupu originálu. Do výšky pak připojte výstup z **Mix color**.
![L10](https://github.com/user-attachments/assets/183f192b-3af4-4fbf-bfdd-a79d031a8871)
</details>

<div align="right">
<a href="https://github.com/Milimar16/Blender-realisticke-povrchy/blob/main/Led%20-%20p%C5%99ehled.md">Další krok =></a>
 </div>
