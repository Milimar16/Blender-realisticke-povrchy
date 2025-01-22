# Hrubost a velké nerovnosti ledu

<details>
<summary>Krok 1. Hrubost</summary>

Hrubost (Roughness) vytvoříme pomocí nové **Textury šumu**. Můžeme ji dokonce využít v základním nastavení, jenom **Detail** nastavte na **maximum**. Také tento uzel připojte za již vytvořený uzel **Mapování**.

Dále z faktorového výstupu textury připojte a vytvořte uzel **Rampa barev** a posuvníky nastavte do 1/3 a 1/2 přičemž nalevo nechte bílou barvu (#ffffff) a napravou tmavší šedou (v ukázce #555555). Barvový výstup rampy připojte do vstupu **Roughness** uzlu Principled BSDF.
![L5](https://github.com/user-attachments/assets/f9734e75-30f5-4a07-b9eb-b56b6fdc3406)

</details>
<details>
<summary>Krok 2. Nerovnosti</summary>

K výraznějším nerovnostím můžeme využít již vytvořenou **Texturu šumu**. Za ni nám stačí připojit druhou **Rampu barev** kde posuvník s černou barvou dejte doprostřed a s tmavě šedou do 9/10 (skoro ke konci).

Tuto **Rampu barev** poté připojte do vstupu výška nového uzlu **Bump**. Jeho sílu nastavte na 0.2 a jeho normálový výstup do normálového vstupu uzlu Bump z předchozí kapitoly.
![L6](https://github.com/user-attachments/assets/1acca53c-092f-458f-bfde-8d61eaeda789)
</details>

<div align="right">
<a href="https://github.com/Milimar16/Blender-realisticke-povrchy/blob/main/%C5%A0kr%C3%A1bance%20ledu.md">Další krok =></a>
 </div>
