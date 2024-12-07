# Kombinace struktur
V této kapitole zkombinujeme 3 struktury asfaltu a to barvu, praskliny a poškození

---
### Krok 1. Ztmavení poškození
Ve stávajícím stavu je štěrk moc světlý na to, aby měl výrazný dopad na vzhled materiálu. Přidejte tedy **Rampu barev** a připojte ji za poslední uzel skupiny, která vytváří poškození. Posuvník černé barvy umístěte dle uvážení.
![A8](https://github.com/user-attachments/assets/4e271d84-c46f-45c5-aa56-f7826cc9db84)

---
### Krok 2. Kombinace
Přidejte do prostředí uzel **Mix color** a zvolte **Ztmavit** jako režim míchání (z prasklin potřebujeme totiž jenom tmavé hodnoty). Do A připojte výstup skupiny uzlů tvořící barvu asfaltu a do B výstup prasklin.
![A9](https://github.com/user-attachments/assets/00f9a7cd-09ef-4187-8012-146073ac2812)

Následně **duplikujte tento uzel** a do nového připojte do A předchozí Mix color a do B výstup rampy barev od prasklin. Výsledek připojte do vstupu Základní barva Principled BSDF a tento uzel do Výstupu materiálu.
![A10](https://github.com/user-attachments/assets/d7a49b87-3f7d-4518-9401-0b66b5528efc)
