---
title: Osoby
layout: single
type: handbook
---

<div style="max-width: 40%;">
  {{< figure src="../../images/entities.png" class="fig-float fig-left" >}}
</div>

{{< intro >}}

Vrstva **Osoby** tvoří jádro každé MemoMapy. Zachycuje jednotlivé místní židovské obyvatele – jejich jména, základní životní údaje a osudy během holokaustu. Každý záznam představuje jednu konkrétní osobu, která v daném městě/obci žila.

V mapové aplikaci se osoby nezobrazují jako samostatné body, ale sdružují se podle **adres domů**, v nichž žily. Uživatel tedy nejprve klikne na dům a teprve v jeho detailu vidí seznam osob, které v něm bydlely, a dále může rozkliknout detail každé osoby zvlášť. Ikona na mapě se proto zobrazuje jako domeček, čílo uvnitř domečku pak zobrazuje, kolik osob na daném místě žilo.
{{< /intro >}}

<div style="margin-top: 4rem;"></div>

## Jaké údaje o osobách evidujeme:

U osob evidujeme pouze takové údaje, které jsou důležité pro porozumění jejich životnímu příběhu a pro jednoznačnou identifikaci. Ne všechny informace musí být k dispozici u všech osob – v řadě případů pracujeme jen s torzovitě dochovanými daty.

Níže jsou shrnuté základní skupiny údajů:

### 1. Základní identifikace osoby

- **Jméno**  
  Dané jméno, případně kombinace prvního a prostředního jména.
- **Příjmení**
- **Rodné příjmení**  
  U vdaných žen uvádíme také rodné příjmení, pokud je známo.  
- **Titul**  
  Akademické nebo jiné tituly před či za jménem (např. „Dr.“, „JUDr.“ apod.).  
- **Pohlaví**  
  Informace o pohlaví osoby, která se využívá např. při formulaci textů v některých částech aplikace.

### 2. Životní data

- **Datum narození**  
  Strukturované datum ve formátu den–měsíc–rok, pokud je známé.  
- **Textový údaj k narození**  
  Pokud přesné datum neznáme (například pouze rok nebo přibližné období), můžeme uvést slovní popis (např. „kolem roku 1890“, „asi 1890–1895“).  
- **Datum úmrtí**  
  Strukturované datum úmrtíve formátu den–měsíc–rok, pokud je známé.  
- **Textový údaj k úmrtí**  
  Pro případy, kdy známe datum jen přibližně nebo jej neznáme celé, můžeme uvést slovní popis (např. „1942“, „léto 1941“, „cca 1942“).   

### 3. Osud během holokaustu

- **Osud**  
  Výběr ze dvou možností z předem připraveného seznamu („zahynul/a“, „přežil/a“). 

### 4. Popis a poznámky

- **Popis**  
  Volný text. Obsahuje veškeré doplnující informace o osobě, které chceme v aplikaci zveřejnit, ale nehodí se do žádného z předchozích strukturovaných údajů nebo vztahového pole. Může obsahovat informace o zaměstnání, o okolnostech deportace či věznění.

- **Poznámky**  
  Volný text. Obsahuje veškeré doplnující informace, které v aplikaci nechceme zveřejnit, ale nechceme na ně při tvorbě aplikace zapomenout. Například „Dva různé údaje o datu úmrtí.“, "Pravděpodobně bratr Terezy Novákové.".
  
<div style="margin-top: 4rem;"></div>

## Vztahy k dalším typům dat v MemoMapě:

Uváděné údaje osoby nemohou být považovány za kompletní, dokud je nepropojíme s dalšími typy dat. Jednotlivé osoby mají vždy vztah minimálně k jednomu dalšímu datovému typu, a to k místu – jen tak dokážeme osobu zanést na mapu (do správného doměčku). Další typy vztahů jsou volitelné, tzn. doplňujeme je pouze v případě, že máme danou informaci k dispozici.

U osob pracujeme s těmito vazbami:

### 1. Vztah k místům

Každá osoba je spojená s jedním nebo více **místy**, kde žila nebo pobývala (místo narození, bydliště před deportací, ale také například místo věznění či úmrtí). U každého takového vztahu můžeme evidovat:

- typ vztahu k místu (např. „poslední bydliště před deportací“, „místo narození“),
- časový rozsah, kdy na daném místě osoba žila (od–do).

Díky tomu lze v mapě zobrazovat osoby v konkrétních domech a zároveň sledovat případné změny adres v čase.

### 2. Vztah k dalším osobám

Dvě osoby mohou být navzájem propojené vztahem:

- rodinnými/příbuzenskými vazbami (rodiče, sourozenci, manželé, děti),  
- ale případně i jiným typem vztahu (spolupracovníci apod.).

V systému je možné takové vazby zaznamenat, aby bylo možné zobrazit celou rodinu nebo skupinu osob, které spolu souvisejí.

### 3. Vztah k datům o transportech

Pokud byla daná osoba deportována do koncentračního tábora či ghetta tzv. hromadným transportem, propojujeme osoby s **údaji o deportaci** prostřednictvím vztahu. Zajímá nás:

- přiřazení ke konkrétnímu transportu, včetně čísla v transportu.


### 4. Vztah k dokumentům a jiným médiím

Naskenované dokumenty, fotografie a případně i další média jsou skvělým doplňkem MemoMapy, který poskytuje další důležité informace o osobě nebo dokonce jejich fotografie. Pokud jsou takováto média k dispozici, je důležité mezi osobou a příslušným médiem vytvořit vztah.

V mapové aplikaci se tyto dokumenty a média zobrazují přímo v detailu osoby a umožňují uživatelům nahlédnout do konkrétních pramenů.

### 5. Vztah k příběhovým mapám

Osoba může být součástí tzv. **příběhové mapy**. Tyto mapy zobrazují trajektorii (trasu) osoby v prostoru a čase a vyprávějí nám její příběh nebo jeho část. Pokud k osobě existuje příběhová mapa, je důležité mezi osobou a příběhovou mapou vytvořit vztah. Aplikace se prostřednictvím tohoto vztahu "dozví", že je příslušná příbehová mapa k dispozici a bude na ni uživatele odkazovat.  
