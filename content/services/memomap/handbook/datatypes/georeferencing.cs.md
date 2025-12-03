---
title: Jak georeferencovat historickou mapu | Návod krok za krokem
layout: single
type: handbook
---

{{< intro >}}
{{< figure src="../../images/georef-1.jpg" class="fig-float fig-right" >}}
Georeferencování je proces, při kterém naskenovanou historickou mapu „připevníme“ k současnému souřadnicovému systému tak, aby ji bylo možné přesně překrýt s dnešní mapou. Tuto část procesu tvorby MemoMapy většinou zajišťuje náš tým v MÚA, ale technicky zdatnější uživatelé georeferencování snadno zvládnou sami.

Pokud si na georeferencování netroufáte, projděte si jen několik úvodních kroků návodu, které se zabývají skenováním a úpravou historické mapy. Naskenovanou mapu nám pak můžete jednoduše předat a georeferencování už zajistíme my.
{{< /intro >}}

<div style="margin-top: 4rem;"></div>

### 1. Skenování historické mapy

Prvním krokem je převést papírovou mapu do digitální podoby.

- **Rozlišení:** Doporučujeme minimálně 600 dpi.  
- **Formát souboru:** Bezztrátový formát (ideálně **TIFF**). Formát JPEG lze použít, ale není tak kvalitní.  
- **Barevnost:** Vždy barevně.  
- **Vícedílné skeny:** Pokud je mapa větší než skener, skenujte ji po částech – vždy ale s přesahem, který usnadní pozdější spojování jednotlivých dílů.

Pokud je mapa křehká nebo svázaná, doporučujeme využít možnost odborného skenování zaměstnanci příslušného archivu nebo muzea.

<div style="margin-top: 4rem;"></div>

### 2. Úprava naskenované mapy

Než začneme mapu georeferencovat, je vhodné ji lehce upravit. Pro úpravu můžeme použít jakýkoli softwar na úpravu obrázků, doporučujeme například [**Gimp**](https://www.gimp.org/downloads/), který je zdarma a nabízí veškeré potřebné funkce.

- **Oříznout okraje:** Papírová mapa obvykle obsahuje okraje s názvem a legendou, nás ale zajímá pouze samotná mapová část – vše ostatní můžeme oříznout.
- **Narovnat sken:** Mapu se většinou nepodaří naskenovat úplně rovně – pomocí softwaru na úpravu obrázků to můžeme napravit.  
- **Rozdělit mapu na části:** Pokud je soubor příliš velký (nad 50 MB), vyplatí se sken rozdělit na několik dílů. Zpracování pomocí specializovaného GIS softwaru pak bude rychlejší a méně náročné.

Upravený obrázek uložíme opět jako TIFF. Pokud obrázek dělíme na více částí, mělo by být z názvů souborů patrné, jak z jednotlivých částí poskládat celou mapu – georeferencování pak bude snadnější.

<div style="margin-top: 4rem;"></div>

### 3. Instalace QGIS

<div style="max-width: 30%; float: right; margin-left: 1rem; margin-bottom: 1rem; ">
  {{< figure src="../../images/qgis-download.JPG" >}}
</div>

Pro georeferencování používáme specializovaný geografický informační systém. [**QGIS**](https://qgis.org/download/) je volně dostupný GIS software a je lokalizovaný do češtiny.

- V dialogovém okně stahování nejprve vyberte operační systém svého počítače. Výchozí nastavení je Windows, pokud používáte ten, nemusíte nic měnit.
- Následně kliknete na verzi softwaru, kterou chcete stáhnout. Doporučujeme stáhnout stabilní verzi **Long Term Release**.  
- Program se instaluje jako jakákoli jiná běžná aplikace.

<div style="margin-top: 4rem;"></div>

### 4. Příprava podkladu v QGIS

Pro georeferencování nejprve potřebujete **moderní mapový podklad**, podle něhož budete zarovnávat sken historické mapy:

<div style="max-width: 45%; float: right; margin-left: 1rem; margin-bottom: 1rem; ">
<a href="../../images/qgis-osm.jpg">
  {{< figure src="../../images/qgis-osm.jpg" >}}
</a>
</div>

- Otevřete QGIS a vytvořte nový projekt: menu na horní liště ->  Projekt -> Nové.
- Projekt hned uložte, abyste něpřišli o svou práci: Projekt -> Uložit jako -> vyberte složku, do níž se projekt uloží, a napište název uloženého souboru -> jako typ souboru nechte *.qgz.
- Přidejte vrstvu současné mapy (doporučujeme OpenStreetMap). Vrstvu přidáme z levého okna s názvem Prohlížeč: volba XYZ Tiles -> OpenStreetMap -> dvakrát kliknout -> mapa se načte v hlavním okně.
- Načtená mapa je oddálená tak, že vidíme celý svět. Mapu můžeme libovolně přiblížit až na detail jednotlivých ulic v našem městě. 

Na tento podklad budeme zarovnávat historickou mapu.

<div style="margin-top: 4rem;"></div>

### 5. Spuštění nástroje pro georeferencování

- V horním menu vyberte **Rastr → Georeferencer**.  
- Otevřete soubor s naskenovanou historickou mapou.  
- Georeferencer zobrazí mapu a umožní vkládat tzv. **vlícovací body**, které historickou mapu zarovnají s mapou současnou.

<div style="display: flex; gap: 1rem; justify-content: space-between; margin-top: 1rem;">

  <div style="flex: 1; text-align: center;">
    <a href="../../images/qgis-georef1.png">
      <img src="../../images/qgis-georef1.png"
           alt="Georeference krok 1"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 1; text-align: center;">
    <a href="../../images/qgis-georef2.png">
      <img src="../../images/qgis-georef2.png"
           alt="Georeference krok 2"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 1; text-align: center;">
    <a href="../../images/qgis-georef3.png">
      <img src="../../images/qgis-georef3.png"
           alt="Georeference krok 3"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

</div>

<div style="margin-top: 4rem;"></div>

### 6. Výběr prvních vlícovacích bodů

Vlícovací body jsou body, které jsou jednoznačně identifikovatelné na historické i moderní mapě.

**Typicky se jedná o:**

- rohy náměstí,
- významné křižovatky,
- kostely, mosty, kapličky,
- původní orientační body (zachovaná uliční síť).

**Postup:**

- Kliknete na vybraný bod na historické mapě.  
- Vyberete odpovídající místo na moderní mapě, na kterou vás QGIS přepne po zvolení možnosti "Z mapového okna".
- Když odsouhlasíte polohu bodu pomocí tlačítka Ok, v tabulce pod georeferencvóvanou mapou se vám objeví souřadnice zapsaného bodu.  
- Opakujete na dalších místech.

**Doporučení:**

- První vlícovací body je vhodné rovnoměrně rozprostřít po mapě (čtyři body na jednom malém náměstí nepomohou s prvotním zarovnáním tak jako čtyři body v rozích mapy).
- Pro první zarovnání vyberte alespoň **4–5 bodů**. Po prvotním zarovnání bude nutné body přidávat. Georeferencování historické mapy je náročně, protože staré mapy většinou nejsou příliš přesné. Finálně tedy mohou být na mapě až stovky jednotlivých vlícovacích bodů.  
- Vyhýbejte se objektům, které se v čase výrazně měnily.
- Využívejte možnosti zvětšení (tlačítko +) historické i moderní mapy, abyste polohu bodů trefili co nejpřesněji.
- Když uděláte chybu, vždycky je možné bod posunou nebo smazat (více níže).

<div style="
  max-width: 820px;
  display: flex;
  gap: 0.7rem;
  justify-content: space-between;
  flex-wrap: nowrap;
  margin-top: 1rem;
">

  <div style="flex: 0 0 18%; text-align: center;">
    <a href="../../images/qgis-georef4.png">
      <img src="../../images/qgis-georef4.png"
           alt="Georeference krok 4"
           style="max-height: 200px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 0 0 18%; text-align: center;">
    <a href="../../images/qgis-georef5.png">
      <img src="../../images/qgis-georef5.png"
           alt="Georeference krok 5"
           style="max-height: 200px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 0 0 18%; text-align: center;">
    <a href="../../images/qgis-georef6.png">
      <img src="../../images/qgis-georef6.png"
           alt="Georeference krok 6"
           style="max-height: 200px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 0 0 18%; text-align: center;">
    <a href="../../images/qgis-georef7.png">
      <img src="../../images/qgis-georef7.png"
           alt="Georeference krok 7"
           style="max-height: 200px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 0 0 18%; text-align: center;">
    <a href="../../images/qgis-georef8.png">
      <img src="../../images/qgis-georef8.png"
           alt="Georeference krok 8"
           style="max-height: 200px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

</div>

<div style="margin-top: 4rem;"></div>


### 7. Nastavení transformace a spuštění georeferencování

Po vložení prvních několika bodů musíme nechat proběhnou proces georeferencování, který podle vybraných bodů na podklad zarovná historickou mapu.

- Klikneme na zelené tlačítko "Spustit georeferencování" v horní liště tlačítek.
- Nastavíme typ a parametry transformace **přesně dle obrázku** níže.

QGIS vytvoří **georeferencovaný GeoTIFF**, který už "ví", kde na mapě leží, a vloží jej přímo do okna mapy, kde můžete zkontrolovat výsledek. Výsledek první transformace s jen několika body nebude dobrý a bude třeba vkládat další vlícovací body stejným způsobem, až dokud výsledek transformace nebude co možná nejvíce přesný.

<div style="display: flex; gap: 1rem; justify-content: space-between; margin-top: 1rem;">

  <div style="flex: 1; text-align: center;">
    <a href="../../images/qgis-georef9.png">
      <img src="../../images/qgis-georef9.png"
           alt="Georeference krok 9"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 1; text-align: center;">
    <a href="../../images/qgis-georef10.png">
      <img src="../../images/qgis-georef10.png"
           alt="Georeference krok 10"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 1; text-align: center;">
    <a href="../../images/qgis-georef11.png">
      <img src="../../images/qgis-georef11.png"
           alt="Georeference krok 11"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

</div>

<div style="margin-top: 4rem;"></div>


### 8. Kontrola výsledku georeferencování a další úpravy

Mapa georeferencovaná podle kroku 7 se automaticky otevře v mapovém okně a my musíme zkontrolovat, zda **překrývá** se současným mapovým podkladem.
 
- Pro snadnější kontrolu je vhodné georeferencovanou mapu "zprůhlednit", aby prosvítal podklad pod ní: pravým tlačítkem myši klikneme na název vrstvy georeferencované mapy v levém okně mapy -> klikneme na Vlastnosti -> Průhlednost -> zvolíme průhlednost okolo 60 % -> tlačítkem Použít otestujeme, zda je průhlednost dostatečná -> průhlednost dále upravíme, nebo necháme tak, jak je -> tlačítkem Ok zavřeme dialog.

<div style="display: flex; gap: 1rem; justify-content: space-between; margin-top: 1rem;">

  <div style="flex: 1; text-align: center;">
    <a href="../../images/qgis-georef12.png">
      <img src="../../images/qgis-georef12.png"
           alt="Georeference krok 12"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 1; text-align: center;">
    <a href="../../images/qgis-georef13.png">
      <img src="../../images/qgis-georef13.png"
           alt="Georeference krok 13"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 1; text-align: center;">
    <a href="../../images/qgis-georef14.png">
      <img src="../../images/qgis-georef14.png"
           alt="Georeference krok 14"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

</div>

- Pokud jsou odchylky velké, upravte nebo doplňte vlícovací body podle kroku 7.
- Někdy je třeba některé vlícovací body posunout nebo smazat. Tlačítka pro smazání a přesunut bodu se nachází v horní tlačítkové liště okna georeferencování: kliknout na příslušné tlačítko -> kliknout na bod na mapě (ten se dle volby buď smaže, nebo je možné jej přesunout). Tlačítko přesouvání bodu umožňuje body přesouvat na historické mapě i na mapě současné.

<div style="display: flex; gap: 1rem; justify-content: space-between; margin-top: 1rem;">

  <div style="flex: 1; text-align: center;">
    <a href="../../images/qgis-georef15.png">
      <img src="../../images/qgis-georef15.png"
           alt="Georeference krok 15"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 1; text-align: center;">
    <a href="../../images/qgis-georef16.png">
      <img src="../../images/qgis-georef16.png"
           alt="Georeference krok 16"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>
</div>

- Průběžně (např. po každých zanesených 5 bodech) spouštějte georeferencování dle bodu 7. Detaily transformace již není nutné znovu zadávat, program si je pamatuje.

Jakmile vše sedí, mapa je připravená pro použití v MemoMapě. Celý proces odtud přebíráme my – vy nám jen zašlete nebo jinak nasdílíte hotovou georeferencovanou mapu. 







