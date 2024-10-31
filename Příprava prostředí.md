# Příprava prostředí
### Krok 1. Konfigurace render engine
**Otevřete na svém počítači Blender** a jako první by jste měli vidět toto základní rozpoložení:
![Základní rozpoložení](https://github.com/user-attachments/assets/1beefad8-bfb7-4aa6-8723-c254f48c9007)
<br>
Dále vyberte v pravé liště možnost **Render** a v první možnosti 
**Render engine** jej změnte z EEVEE na **Cycles**.
<br>
<div align="center">
<img
  src="https://github.com/user-attachments/assets/ac61b7ed-f462-429e-81e8-172bc7a10fe2"
  alt="Renderovací konfigurace"
  width="75%"
  align="middle"
/> </div>
<br>
Tímto krokem jste změnili render engine, který bude blender využívat. Cycles je vhodnější pro renderování realismu. Je ale hardwarově více náročný proto se nedivte, když váš render nebude trvat pár sekund jako v EEVEE, ale několik minut (a nebo hodin 😱 u náročnějších scén!)

-------

### Krok 2. Instalace rozšíření [Node Wrangler](https://docs.blender.org/manual/en/latest/addons/node/node_wrangler.html) a [Material Library](https://projects.blender.org/extensions/materials_library_vx)
_Pokud již máte tato rozšíření aktivována, přeskočte tento krok._

Otevřete v horní liště možnost **Upravit** a zvolte **⚙️ Předvolby...** (alternativně můžete zmáčnkout klávesy **Ctrl + ,**)
<div align="center">
<img
  src="https://github.com/user-attachments/assets/70fe738c-c03a-4219-b33e-87aa207ca570"
  alt="Předvolby"
  width="75%"
  align="middle"
/> </div>
<br>

V následujícím okně vyberte na levé straně záložku **Rozšíření** a tam vyhledejte a následně zaklikněte rozšíření **Node Wrangler**. 
<br>
<div align="center">
<img
  src="https://github.com/user-attachments/assets/95433d28-5ea3-4857-8766-19f26919ced8"
  alt="Předvolby"
  width="75%"
  align="middle"
/> </div>
<br>

Toto rozšíření umožňuje příjemnější práci s uzly (nodes) v dalších krocích.
<br>

Potom ve stejém okně vyberte záložku **Get Extensions** a zde vyhledejte a **nainstalujte** (tlačítkem _install_) rozšíření **Material Library**.
<div align="center">
<img
  src="https://github.com/user-attachments/assets/631d54a0-43fe-4e2b-9a20-2b2948be4d60"
  alt="Předvolby"
  width="75%"
  align="middle"
/> </div>
<br>

Toto rozšíření umožňuje ukládání materiálů a jejich používání napříč různými projekty.
<br>

Následně ve vrchní liště vyberte **Shading**, a nový materiál se vám sám vytvoří.
Teď už je váš program připraven a můžeme se pustit do tvorby materiálů!

