# Velké škrábance

<details>
<summary>Krok 1. - Vytvoření textury pomocí 2 uzlů</summary>

#### a) Vlnová textura
Pomocí tohoto uzlu určíme tvar a všeobecný vzhled škrábanců.

Připojte nový uzel **Vlnová textura** za Mapování a upravte jej následujícím způsobem:
- **Velikost** nastavte na cca 3.5, toto určuje velikost a frekvenci škrábanců.
- **Historii vracení** na asi 4, toto určuje zkreslení a kroucení škrábanců.
- **Detail Roughness** na maximum.

_Doporučuji si pohrát s uzlem mapování (přesněji s rotací) aby vaše textura nevypadala jako na prvním obrázku. Toto se samozřejmě vztahuje jen na krychle a podobné objekty. __Dejte ale pozor na to že pokud cokoliv upravíte v Mapování, všechny uzly závislé na tomto se také ovlivní!___
![O8](https://github.com/user-attachments/assets/060abe2e-5a1e-4ea9-a352-0097eb73e9ac)

#### b) Textura šumu
Pomocí tohoto uzlu určíme oblast ve které se budou škrábance projevovat.

Vytvořte nový uzel **Textura šumu**, který zatím nechte volně v prostoru, nastavte typ šumu na **Hetero Terrain** upravte jej následujícím způsobem:
- **Velikost** nastavte na cca 1.4, toto určuje velikost oblastí.
- **Detail** na maximum.
- **Historie vracení** na 1 - 4, toto určuje nepravidelnost a rozpoložení oblastí.
Náhled na tuto texturu by měl vypadat asi takto:
<div align="center">
<img
  src="https://github.com/user-attachments/assets/97d8a423-1e23-4494-8e42-f43dc20c74ce"
  alt="O9"
  width="50%"
  align="middle"
/> </div>
<br>

</details>
<details>

<summary>Krok 2. - Sloučení 2 textur</summary>

To aby se Vlnová textura projevovala v oblastech určených Texturou šumu, využijeme uzly **Oddělit XYZ** a **Kombinovat XYZ**. Poté přiřadíme Vlnovou texturu pouze k jedné ze souřadnic (v tomto případě **Y**), ostatní necháme být.

Vytvořte tyto dva uzly a připojte je následovně:
<div align="center">
<img
  src="https://github.com/user-attachments/assets/2ff93dec-53be-4914-a4af-3c51807f0961"
  alt="O10"
  width="50%"
  align="middle"
/> </div>
<br>

Tímto se nám spojily tyto dvě textury, a škrábance se budou projevovat více na oblastech vyznačených Texturou šumu.

</details>
<details>

<summary>Krok 3. - Omezení rozsahu a spojení s ostatními normálami</summary>

V této podobě by byly škrábance příliš časté a ostré, proto přidáme za Texturu šumu ještě **Rampu barev** u které posunutím posuvníků dosáhneme přesně toho (ještě nezapomeňte prohodit bílou a černou).
<div align="center">
<img
  src="https://github.com/user-attachments/assets/11412d86-c454-4b37-bc4e-833d8336e584"
  alt="O10"
  width="50%"
  align="middle"
/> </div>
<br>

Teď už nám stačí pouze zkombinovat tuto normálovou mapu s ostatními dvěma vytvořenými v minulých kapitolách, a to zase za pomocí uzlu **Bump**, do jekož vstupu Výška zapojíme naši novou texturu, a do Normály připojíme výstup minulého Bump uzlu.

Duplikujeme tedy minulý **Bump** uzel (Shift + D) a připojíme jej tak jak bylo popsáno, s výstupem vedoucím do vstupu Normála na uzlu **Principled BSDF**.

![O12](https://github.com/user-attachments/assets/f2c034eb-1baf-437f-a421-3a3733503eb1)

Nakonec nezapomeňte připojit Principled BSDF s výstupem, jako na obrázku.
</details>

<div align="right">
<a href="https://github.com/Milimar16/Blender-realisticke-povrchy/blob/main/Ocel%20-%20p%C5%99ehled.md">Další krok =></a>
 </div>
