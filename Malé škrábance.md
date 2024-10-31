# Malé škrábance oceli
### Krok 1. - Vytvoření normálové mapy škrábanců
Přidejte do prostředí uzel **Textura šumu**, kterou připojte rovnou za uzel Mapování, a **Rampu barev**.
**Texturu šumu** upravte takto:
- **Velikost** nastavte na cca 4
- **Detail** na maximum
- **Roughness** na cca 0.5
- **Historii vracení** na vysokých 13 až 19, aby škrábance tvořily linie, které vedou do všech směrů.
<br>

Za ní připojte **Rampu barev**, kde na levé straně nastavte černou, na pravé bílou a posuvníky přibližte k sobě, čímž omezíte plochu škrábanců a zdůrazníte jejich hloubku.
Pak spojte následovně (obrázek ukazuje náhled na uzel Rampa barev):
<div align="center">
<img
  src="https://github.com/user-attachments/assets/645a7eeb-b89b-4243-a328-b54c0a339d70"
  alt="O4"
  width="75%"
  align="middle"
/> </div>

---

### Krok 2. - Spojení normálových map škrábanců a zrna
Spojení této a minulé hrubosti zrna dosáhneme dalším **Bump** uzlem. Můžeme duplikovat předchozí, zapojit do výšky naši nynější texturu a do normály připojit předchozí Bump uzel.
<br>
<br>
_Před zapojením:_
<div align="center">
<img
  src="https://github.com/user-attachments/assets/23ad69a7-c649-4854-a1a6-47376d8392db"
  alt="O5"
  width="75%"
  align="middle"
/> </div>
<br>

_Po zapojení:_
<br>
<div align="center">
<img
  src="https://github.com/user-attachments/assets/f61cefdf-c173-45ce-8734-e153aaa0fcae"
  alt="O6"
  width="75%"
  align="middle"
/> </div>
<br><br>
Výsledkem by měla být textura na které je vidět jak zrno (červeně vyznačeno) tak menší škrábance (zeleně vyznačeno): <br><br>
<div align="center">
  
![O7](https://github.com/user-attachments/assets/bfdd193b-e228-4ccb-8d49-16b548e6ce8c)
</div>
