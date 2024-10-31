# Zrno oceli
### Krok 1. - Úprava Principled BSDF
Potažením myší posuňte hodnotu metalýzy **(Metallic)** na maximum, tedy 1. 
![Metallic](https://github.com/user-attachments/assets/dd76c2fa-31bf-4309-9696-27e3896cab9c)
<br>
A stejným způsobem snižte **Roughness** někam mezi 0.4 a 0.2.
### Krok 2. - Přidání zrnění pomocí vlnové textury
Přidejte do prostředí uzel **Vlnová textura** (zmáčknutím Shift + A) a poté ji vyberte a stiskněte Ctrl a T, toto přidá uzly Mapování a Souřadnice textury, které se budou hodit následovně.
Také propojte výstup Objekt v Souřadnici textury s Vektorem v Mapování, toto materiálu dovolí lepší rozložení po povrchu objektu.
![Vlnova_textura](https://github.com/user-attachments/assets/aab41700-6fec-4611-91ef-71c81b688845)
<br>

_Kliknutím na jakýkoliv uzel levým tlačítkem se stisknutými Ctrl a Shift se vám ukáže náhled daného uzlu._
<br>
_Spojení mezi uzly přeříznete tím, že se stisknutým Ctrl přetáhnete pravým tlačítkem myši přes křivku._
<br> <br>

Upravte uzel Vlnové textury následujícím způsobem:
- **Velikost** snižte přibližně na 0.1
- **Historii vracení** navyšte na cokoliv mezi 60 a 100
- **Detail** dejte na maximum
- **Detail Roughness** na přibližně 0.7
<br>

S těmito úpravami by náhled uzlu měl vypadat asi takto:
<div align="center">
<img
  src="https://github.com/user-attachments/assets/36684899-aae6-4355-9d65-778b4c2223dd"
  alt="O1"
  width="75%"
  align="middle"
/> </div>
<br>

Přidejte mezi Vlnovou texturu a Principled BDSF **Rampu barev** a nastavte obě barvy na velmi podobné šedé, aby nebyl kontrast moc velký. <br>
Následně propojte takto:
<div align="center">
<img
  src="https://github.com/user-attachments/assets/5f8c6350-4140-4bb4-9811-7d9dad400dc4"
  alt="O2"
  width="75%"
  align="middle"
/> </div>

### Krok 3. - Přidání výstupků zrnění
Vytvořte 2 další uzly a to **Bump**, který konvertuje na normálové nerovnosti, a další **Rampu barev**, která bude ovlivňovat míru pokrytí povrchu.
<br>

**Bump** nastavte tak - aby síla byla velmi nízká (něco mezi 0.02 a 0.05) a v <br>

**Rampě barev** - prohoďte potažením posuvníků černou s bílou a nastavte bílou na přibližně 0.75 a černou na 1 <br><br>

Poté zapojte následovně, aby se bump projevil jako výstupky na výsledném zrnění kovu:
<div align="center">
<img
  src="https://github.com/user-attachments/assets/5e0ccba2-679b-4619-a35e-a1c44c50bac4"
  alt="O3"
  width="75%"
  align="middle"
/> </div>
<div align="right">
<a href="https://github.com/Milimar16/Blender-realisticke-povrchy/blob/main/Mal%C3%A9%20%C5%A1kr%C3%A1bance.md">Další krok =></a>
 </div>
