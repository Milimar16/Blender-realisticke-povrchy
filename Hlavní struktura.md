# Hlavní struktura
### Krok 1. Příprava texturových uzlů
Vložte do prostředí 2 **Textury šumu**. První (vyznačena v obrázku zeleně) bude sloužit podobně jako Musgrave textura z verze Blenderu 4.0, takže ji nastavte následovně:
- **Velikost** na 2
- **Detail** na maximum
- **Roughness** na maximum
- **Lacunarity** na přibližně 2.8
- **Zakažte** možnost **Normalizovat**

Druhá Textura šumu (vyznačena červeně) bude standardní texturou, která bude tvořit jakési "rozmazané vlnění" nutné pro vzhled dřeva. Tu nastavte takto:
- **Velikost** snižte na 2.5
- **Detail** na maximum
- **Historii vracení** na cokoliv mezi 1 a 2, záleží jak strukturované jej chcete mít (v ukázce 1.3)

![D1](https://github.com/user-attachments/assets/fac64d61-c1d0-40b3-ae44-6112a745b713)

---
### Krok 2. Mapování textury
Před smícháním obou textur nejdříve musíme ovlivnit jejich mapování a to pomocí uzlu **Mapování**. Nejdříve vložte uzel **Mix Color** do roviny, vyberte jej a zmáčkněte **Ctrl + T**. Měly by se vám zjevit 3 nové uzly, Souřadnice textury, Mapování a Obrázková textura, tento poslední smažte (vyberte jej a zmáčněte Delete nebo Ctrl + X).

Následně přepojte výstup **Objekt** ze Souřadnic textury do vstupu Vektor v Mapování a **Vektorový výstup** mapování do prvního (**A**) vstupu **Mix** uzlu.

![D2](https://github.com/user-attachments/assets/ccc00af5-d05f-4ad1-a9e2-401bbd88ee19)

Následně snižte dvě z dimenzí (nejlépe Y a Z) v záložce Velikost v uzlu Mapování na **0.15**. Tímto dosáhnete protáhlejší textury jaká je právě v tečnovém řezu dřeva.

---
### Krok 3. Míchání textur
Dalším krokem bude kombinace daných textur pomocí uzlů **Mix**. Ten, jenž jste vložili v minulém kroku, připojte k normalizované textuře šumu (vstup vektor).

![D3](https://github.com/user-attachments/assets/c6bced4c-a6d7-4ae4-965d-7cc1fb0953b3)

Následně přidejte druhý uzel **Mix color**, a nastavte jej na cca 0.75. Právě tento bude míchat textury. Do vstupu A pak připojte faktorový (fac) výstup nenormalizované Textury šumu a do B faktorový výstup normalizované Textury šumu.
Také připojte faktorový výstup normalizované textury šumu do vektorového vstupu nenormalizované, což zkroutí detaily dle první textury.

_Pro zjednodušení jsou uzly šumu ohraničeny stejnými barvami jako v prvním kroku._
![D4](https://github.com/user-attachments/assets/76e9697d-7c9b-4329-98c3-95beced9afb9)

---
### Krok 4. Zbarevnění
Posledním krokem této části bude zbarevnění (aby dřevo nebylo jen černobílé). Tohoto dosáhneme přidáním **Rampy barev** za výstup druhého mixovacího uzlu a před vstup **Základní barva** v Principled BSDF.
Do Rampy barev pomocí tlačítka **+** přidejte jeden nebo dva další posuvníky, přičemž barvy na těchto posuvnících vyberte od vámi určené nejtmavší hnědé po nejsvětlejší béžovou, a tyto dva extrémy umístěte na kraje gradientového řádku.

_Příklad barevného provedení (podle autorovy kuchyňské linky):_
![D5](https://github.com/user-attachments/assets/d3024f97-c0ce-4f83-b945-1eda7dfe7d0d)

