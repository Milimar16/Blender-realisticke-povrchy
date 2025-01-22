# Barva asfaltu

<details>
<summary>Krok 1. Textura Voronoi</summary>

Základní texturovou složkou barvy samotného asfaltu bude **Textura Voronoi**. Přidejte tento uzel do prostředí a upravte jej následovně:
- Feature output na **Smooth F1** namísto jednoduchého F1
- Změňte metriku vzdálenosti textury na typ **Minkowski** z Euklidovského
- **Velikost** na 10
- **Exponent** na maximum
</details>
<details>

<summary>Krok 2. Zkreslení textury</summary>

Zkreslení Textury Voronoi dosáhneme pomocí uzlu **Textury šumu**. Přidejte do prostředí tento uzel a upravte jej takto:
- **Velikost** na 18
- **Detail** na maximum

Ještě uzel ale nepřipojujte k prvnímu, protože výsledné zkreslení by bylo moc silné. Přidejte proto uzel **Mix color**, změňte Blending mode (míchací režim) na Lineární světlo aby úpravy byly rovnoměrné a Faktor na 0.1.

Následně připojte Texturu šumu do vstupu B a do vstupu A připojte uzel **Souřadnice textury**, který vytvořte a použijte výstup Objekt. Tento nový uzel také stejným výstupem připojte k Textuře šumu aby bylo rozložení textury rovnoměrné.

Teď už můžete připojit výsledek Mix color do Vektoru Textury Voronoi.
![A1](https://github.com/user-attachments/assets/e9834dbe-f9bc-4828-8f10-db828b817924)
</details>
<details>

<summary>Krok 3. Určení barev</summary>

Určení samotných barev materiálu provedeme jednoduše pomocí uzlu **Rampa barev**, který připojíme za Texturu Voronoi a vstup Základní barva uzlu Principled BSDF. Stačí nastavit okrajové barvy na odstíny šedé.
![A2](https://github.com/user-attachments/assets/fa924eab-ae0f-4f8e-a6c4-0d454b1ae53f)
</details>

<div align="right">
<a href="https://github.com/Milimar16/Blender-realisticke-povrchy/blob/main/Praskliny.md">Další krok =></a>
 </div>
