# Poškození
V této části vytvoříte malé oblasti, na kterých bude vidět štěrk v poškozeních částech asfaltu.

---
### Krok 1. Kamínky
Strukturu jednotlivých kamínků ve štěrku dosáhneme pomocí další **Textury Voronoi** nastavenou na tyto hodnoty:
- **Dimenzi** na 4D (Dosáhneme tím i tmavějších oblastí)
- **Feature output** na Distance to Edge
- **Velikost** na 100

Následně pro slabé zkreslení využijeme znovu **Textury šumu**, kde nastavíme **Detail** na maximum a **Velikost** na 20. Pak vytvořte uzel **Mix color**, jehož Míchací režim vyberte na Lineární světlo, Faktor na 0.3 a do barvy A připojte výstup Objekt uzlu Souřadnice textury a do B samotnou **Texturu šumu**.

Výstup míchacího uzlu připojte k uzlu **Textura Voronoi** a nakonec ještě jednou výstup Objekt připojte i k Vektoru **Textury šumu**.
![A5](https://github.com/user-attachments/assets/56768842-a49c-409a-8277-b32edd9f7213)
