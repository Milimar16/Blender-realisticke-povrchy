# Poškrábaná ocel
### Krok 1. - Upravte Principled BSDF
Potažením myší posuňte hodnotu metalýzy **(Metallic)** na maximum, tedy 1. 
![Metallic](https://github.com/user-attachments/assets/dd76c2fa-31bf-4309-9696-27e3896cab9c)
<br>
A stejným způsobem snižte **Roughness** někam mezi 0.4 a 0.2.
### Krok 2. - Přidejte zrnění pomocí vlnové textury
Přidejte do prostředí uzel **Vlnová textura** (zmáčknutím Shift + A) a poté ji vyberte a stiskněte Ctrl a T, toto přidá uzly Mapování a Souřadnice textury, které se budou hodit následovně.
Také propojte výstup Objekt v Souřadnici textury s Vektorem v Mapování, toto materiálu dovolí lepší rozložení po povrchu objektu.
![Vlnova_textura](https://github.com/user-attachments/assets/aab41700-6fec-4611-91ef-71c81b688845)
<br>

_Kliknutím na jakýkoliv uzel levým tlačítkem se stisknutými Ctrl a Shift se vám ukáže náhled daného uzlu_
<br> <br>

Upravte uzel Vlnové textury následujícím způsobem:
- **Velikost** snižte přibližně na 0.1
- **Historii vracení** navyšte na cokoliv mezi 60 a 100
- **Detail** dejte na maximum
- **Detail Roughness** na přibližně 0.7
<br>

S těmito úpravami by náhled uzlu měl vypadat asi takto:
![O1](https://github.com/user-attachments/assets/36684899-aae6-4355-9d65-778b4c2223dd)

