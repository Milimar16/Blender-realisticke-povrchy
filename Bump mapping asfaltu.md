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

Faktor druhého nastavte na 0.2 a do jeho vstupu Výška připojte výstup 
