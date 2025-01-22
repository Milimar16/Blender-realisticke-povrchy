# Rýhy

<details>
<summary>Krok 1. Textura rýh</summary>

Přidejte další **Textruru šumu** a nastavte:
- **Velikost** a **Detail** na 15
- **Lacunarity** na 2.5

Následně přidejte Mapování a Souřadnice textury a v Mapování Velikost X nastavte na 100. Tímto vyostříte linie rýh.

![D8](https://github.com/user-attachments/assets/cd84f1bd-22a8-4413-8253-a2c0822b50ad)
</details>
<details>

<summary>Krok 2. Omezení výskytu a připojení do barvové sekvence</summary>

Přidáním **Rampy Barev** za texturu šumu a posunutím černého posuvníku cca do poloviny omezíte výskyt škrábanců. Pak vytvořte další **Mix color**, nastavte jej na Násobit a rampu do vstupu A zapojte. Do vstupu B připojte výsledek barevné Rampy Barev z předešlých kapitol.
Výsledek násobícího uzlu připojte do vstupu **Základní barva** (vytváříme tedy jenom barevný základ) uzlu **Principled BSDF**.

![D9](https://github.com/user-attachments/assets/4d89591b-9f88-48e0-a10b-826316ed1b93)
</details>
<details>

<summary>Krok 3. Užití bump mappingu</summary>

Vložte 2 uzly **Bump** a snižte jejich sílu na 0.2. Následovně do Výšky prvního zapojte výstup **Rampy barev** určující barvu dřeva, a do Výšky druhého výstup **Rampy barev** určující rozprostření rýh. 
Propojte normálovými spoji první s druhým a výstup druhého zapojte do **Normály Principled BSDF**.

![D10](https://github.com/user-attachments/assets/33f73781-b80c-4569-9c9f-07115367a565)
</details>


<div align="right">
<a href="https://github.com/Milimar16/Blender-realisticke-povrchy/blob/main/D%C5%99evo%20-%20p%C5%99ehled.md">Další krok =></a>
 </div>
