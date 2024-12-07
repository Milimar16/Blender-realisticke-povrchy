# Bump mapping asfaltu
V této kapitole dáme materiálu hrubost a nerovnosti pomocí uzlů **Bump**.
### Krok 1. Celoplošné nerovnosti
Vytvořte uzel **Textura šumu**, který bude určovat výšku celoplošných nerovností a nastavte takto:
- **Velikost** na cca 55
- **Detail** na maximum
Do vektoru tohoto uzlu použijte zase výstup Objekt Souřadnic textury.

---
### Krok 2. Řetěz uzlů Bump
Pro vytvoření normálové mapy (určení nerovností na materiálu) budeme potřebovat konvertor z barevných hodnot na normálové hodnoty. Tohoto dosáhneme pomocí uzlu **Bump**. Abychom zakomponovali všechny druhy struktur, vytvoříme řetěz těchto uzlů.

Do vstupu Výška prvního z nich připojte Texturu šumu z minulého kroku a poslední připojte do vstupu Normála uzlu Principled BSDF.
![A11](https://github.com/user-attachments/assets/66b6faab-e1ee-4cc9-ab52-3770675c2971)

Faktor druhého nastavte na 0.2 a do jeho vstupu Výška připojte výstup Vzdálenost uzlu Textura Voronoi z první kapitoly ([Barva asfaltu](https://github.com/Milimar16/Blender-realisticke-povrchy/blob/main/Barva%20asfaltu.md)).

Faktor třetího nastavte na 0.3 a do jeho vstupu Výška připojte nový uzel **Rampa barev**, který bude omezovat důraz prasklin. Posuvník bílé dejte téměř doleva. Pak do této rampy barev připojte výstup uzlu **Mix color** z druhé kapitoly ([Praskliny](https://github.com/Milimar16/Blender-realisticke-povrchy/blob/main/Praskliny.md)).
![A12](https://github.com/user-attachments/assets/6c5b6e71-d7f0-4ed3-9e2e-d61726a6b98e)

_V tomto náhledu třetího uzlu Bump byly předešlé dva utlumeny klávesou M_

Faktor čtvrtého nastavte na 0.4 a do jeho vstupu Výška připojte výsledek uzlu **Mix color** z třetí kapitoly ([Poškození](https://github.com/Milimar16/Blender-realisticke-povrchy/blob/main/Po%C5%A1kozen%C3%AD.md)).
![A13](https://github.com/user-attachments/assets/b4b44bd8-4fc1-4a89-b649-596594210e6b)

---
### Krok 3. Hrubost
Konečným krokem bude ovlivnění hrubosti (Roughness) asfaltu. Budeme vycházet z výstupu skupiny uzlů určujících barvu a přidáme do prostředí **Rampu barev** do jejíhž vstupu bude směřovat výstup Vzdálenost uzlu Textura Voronoi z první kapitoly ([Barva asfaltu](https://github.com/Milimar16/Blender-realisticke-povrchy/blob/main/Barva%20asfaltu.md)). Černou barvu na levé straně rampy nahraďte za velmi světlou šedou, aby byl materiál výrazně hrubý. Výstup rampy barev pak povede přímo do vstupu **Roughness** uzlu Principled BSDF.
![A14](https://github.com/user-attachments/assets/915529ec-f859-4552-807f-15350d7e8da2)

<div align="right">
<a href="https://github.com/Milimar16/Blender-realisticke-povrchy/blob/main/Asfalt%20-%20p%C5%99ehled.md">Další krok =></a>
 </div>
