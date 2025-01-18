# Praskliny
### Krok 1. Struktura
Také tato struktura bude založena na **Textuře Voronoi** a jejím zkreslením pomocí **Textury šumu**. Přidejte je tedy do prostředí a Feature output Textury Voronoi změňte na **Distance to Edge** a **Velikost** Textury šumu na 2.5. Následně propojte takto (nezapomeňte na připojení se Souřadnicemi textury):

![A3](https://github.com/user-attachments/assets/7dada819-5261-4727-b13c-97e9d95fe838)

---
### Krok 2. Maska
Aby se praskliny nerozprostírali po celé ploše objektů, použijeme masku, která je omezí.

Duplikujte tedy **Texturu šumu** a za ni připojte **Rampu barev** kde posuvník s černou barvou umístěte přibližně doprostřed. Následně stačí vytvořit další uzel **Mix color** kde do Faktoru připojte výstup Barva z Rampy barev a do vstupu A výstup Textury Voronoi. Barvu B nastavte na bílou (#FFFFFF)

![A4](https://github.com/user-attachments/assets/7a093dfe-94d4-475e-8ead-ba332324adee)

<div align="right">
<a href="https://github.com/Milimar16/Blender-realisticke-povrchy/blob/main/Po%C5%A1kozen%C3%AD.md">Další krok =></a>
 </div>
