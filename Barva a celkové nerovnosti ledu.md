# Barva a celkové nerovnosti ledu

<details>
<summary>Krok 1. Určení základních vlastností v Principled BSDF</summary>

Led má vcelku rozdílné vlastnosti od ostatních materiálů v tomto návodu. Například jeho barvu můžeme zvolit jednoduše pomocí uzlu Principled BSDF a to na slabý odstín modré (v příkladu využita barva #C3D2F5)
![L1](https://github.com/user-attachments/assets/98f0bbdb-5de5-492d-9081-222c87a34044)

Také je narozdíl od ostatních průhledný, toto nastavíme posuvníkem pod záložkou **Průsvitnost** v Principled BSDF na **0**. Následně také nastavte index refrakce **IOR** na **1.3**. Tato vlastnost ovlivňuje jak se světlo odráží a láme na povrchu.
![L2](https://github.com/user-attachments/assets/1ac6067e-c634-4404-b9d5-030b296a78cc)
</details>
<details>
<summary>Krok 2. Přidání mapy celoplošných nerovností</summary>

Celkové nerovnosti přidáme pomocí uzlu **Textura šumu**. Přidejte ji tedy do roviny a za účelem jemného šumu upravte následovně:
- **Velikost** na 1
- **Detail** na maximum

Přidejte (pomocí Ctrl + T) také uzly **Mapování** a **Souřadnice textury** kde vyměňte výstup Generated na **Objekt**.
![L3](https://github.com/user-attachments/assets/804fd68b-4285-4c89-b037-75cd2bc1cbcb)

</details>
<details>

<summary>Krok 3. Konverze na normálové hodnoty</summary>

K tomuto použijeme uzel **Bump**. Přidejte jej a do výšky připojte faktorový výstup Textury šumu. Sílu uzlu nastavte na 0.05 (slabé nerovnosti) a připojte jej do normálového vstupu Principled BSDF.
![L4](https://github.com/user-attachments/assets/0ce3190a-78b6-4233-87c6-145504154a9c)
</details>

<div align="right">
<a href="https://github.com/Milimar16/Blender-realisticke-povrchy/blob/main/Hrubost%20a%20velk%C3%A9%20nerovnosti%20ledu.md">Další krok =></a>
 </div>
