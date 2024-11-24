# Rýhy
### Krok 1. Textura rýh
Přidejte další **Textruru šumu** a nastavte:
- **Velikost** a **Detail** na 15
- **Lacunarity** na 2.5

Následně přidejte Mapování a Souřadnice textury a v Mapování Velikost X nastavte na 100. Tímto vyostříte linie rýh.

![D8](https://github.com/user-attachments/assets/cd84f1bd-22a8-4413-8253-a2c0822b50ad)

---
### Krok 2. Omezení výskytu a připojení do barvové sekvence
Přidáním **Rampy Barev** za texturu šumu a posunutím černého posuvníku cca do poloviny omezíte výskyt škrábanců. Pak vytvořte další **Mix color**, nastavte jej na Násobit a rampu do vstupu A zapojte. Do vstupu B připojte výsledek barevné Rampy Barev z předešlých kapitol.
Výsledek násobícího uzlu připojte do vstupu **Základní barva** (vytváříme tedy jenom barevný základ) uzlu **Principled BSDF**.

![D9](https://github.com/user-attachments/assets/4d89591b-9f88-48e0-a10b-826316ed1b93)
