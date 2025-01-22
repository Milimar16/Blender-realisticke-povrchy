# Poškození
V této části vytvoříte malé oblasti, na kterých bude vidět štěrk v poškozeních částech asfaltu.

<details>

<summary>Krok 1. Kamínky</summary>

Strukturu jednotlivých kamínků ve štěrku dosáhneme pomocí další **Textury Voronoi** nastavenou na tyto hodnoty:
- **Dimenzi** na 4D (Dosáhneme tím i tmavějších oblastí)
- **Feature output** na Distance to Edge
- **Velikost** na 100

Následně pro slabé zkreslení využijeme znovu **Textury šumu**, kde nastavíme **Detail** na maximum a **Velikost** na 20. Pak vytvořte uzel **Mix color**, jehož Míchací režim vyberte na Lineární světlo, Faktor na 0.3 a do barvy A připojte výstup Objekt uzlu Souřadnice textury a do B samotnou **Texturu šumu**.

Výstup míchacího uzlu připojte k uzlu **Textura Voronoi** a nakonec ještě jednou výstup Objekt připojte i k Vektoru **Textury šumu**.
![A5](https://github.com/user-attachments/assets/56768842-a49c-409a-8277-b32edd9f7213)
</details>
<details>

<summary>Krok 2. Maska</summary>

Stejně jako s prasklinami, i zde nechceme aby štěrk pokrýval celou plochu objektu, ale jenom dané části. Duplikujte tedy uzel **Textura šumu** z minulého kroku a snižte **Velikost** na 3.

Potom přidejte **Rampu barev**, kde posuvníky posuňte vcelku hodně k sobě přibližně do 2/5 lišty (můžete i do jiné části, záleží na tom jak moc chcete aby byl váš asfalt poškozen). Do Faktoru zapojte faktorový výstup nové **Textury šumu**.
![A6](https://github.com/user-attachments/assets/5c34ac53-41db-41a3-8a8c-a5bb44ee7dd2)

_Černou jsou vyznačeny budoucí poškozené oblasti._

Stejně jako minulou Texturu šumu i tuto připojte k Souřadnicím textury.

Poslední částí je přidání míchacího uzlu **Mix color**. Faktor nastavte na 1 a do barvy A připojte Texturu Voronoi tvořící kamínky z prvního kroku a do B Rampu barev.

Jelikož chceme jen světlé hodnoty kamínků v poškozených částech, změňte **Blending mode** uzlu Mix color na **Zesvětlit**.
![A7](https://github.com/user-attachments/assets/77ebcfa2-9af2-481b-b60d-b5878c7fab72)

<div align="right">
<a href="https://github.com/Milimar16/Blender-realisticke-povrchy/blob/main/Bump%20mapping%20a%20hrubost%20asfaltu.md">Další krok =></a>
 </div>
