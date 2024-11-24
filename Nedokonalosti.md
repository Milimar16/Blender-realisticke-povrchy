# Nedokonalosti
### Krok 1. Tvorba černobílé mapy pomocí textur
Přidejte do plochy uzel **Vlnová textura** a **Textura šumu**. Nastavte je takto:
**Vlnová textura:** (Tato textura bude zkreslovat následný šum)
- **Velikost** na 0.8
- **Historie vracení** na 4.5
- **Detail** na 1.4
- **Detail scale** na 5
- Směr vln změňte z **X na Y**

**Textura šumu:**
- **Detail** na maximum
- **Lacunarity** na 3.6

Následně zapojte barvový výstup vlnové textury do vektoru Textury šumu a přidejte (pomocí Ctrl + T) Mapování a Souřadnice textury.

![D6](https://github.com/user-attachments/assets/d7387dce-a3f6-445a-a14f-5fbd5cf6ce2d)

---
### Krok 2. Přidání do barevné sekvence
Vytvořte uzel **Rampa barev** kde úplně na kraj levé strany gradientového řádku zvolte čistě bílou barvu a přibližně do 3/5 dejte druhý posuvník se světlou šedou. Toto zjemní efekt textury. Následně výstup této rampy připojte do vstupu A nově vytvořeného uzlu **Mix color**, a do B výstup konečného mixu barev z minulé kapitoly. Zvolte potom místo možnosti **Mix** na **Násobit** a připojte jej do Rampy barev tvořící barvu dřeva.

![D7](https://github.com/user-attachments/assets/f0db0f10-7143-4791-812d-ad8d5306e500)

