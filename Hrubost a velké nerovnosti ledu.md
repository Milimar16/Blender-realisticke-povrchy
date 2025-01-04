# Hrubost a velké nerovnosti ledu
### Krok 1. Hrubost
Hrubost (Roughness) vytvoříme pomocí nové **Textury šumu**. Můžeme ji dokonce využít v základním nastavení, jenom **Detail** nastavte na **maximum**. Také tento uzel připojte za již vytvořený uzel **Mapování**.

Dále z faktorového výstupu textury připojte a vytvořte uzel **Rampa barev** a posuvníky nastavte do 1/3 a 1/2 přičemž nalevo nechte bílou barvu (#ffffff) a napravou tmavší šedou (v ukázce #555555). Barvový výstup rampy připojte do vstupu **Roughness** uzlu Principled BSDF.
![L5](https://github.com/user-attachments/assets/f9734e75-30f5-4a07-b9eb-b56b6fdc3406)
