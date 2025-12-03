---
title: Místa
layout: single
type: handbook
---

<div style="max-width: 40%;">
  {{< figure src="../../images/places.png" class="fig-float fig-left" >}}
</div>

{{< intro >}}

**Místa** představují technický datový typ, který propojuje všechny prvky mapových vrstev s konkrétní polohou na mapě.  
Na rozdíl od ostatních typů dat tvořících mapové vrstvy (osoby, body zájmu, místa paměti, incidenty, události) **nejsou Místa samostatnou vrstvou**, ale slouží jako **referenční bod pro zobrazení na mapě**.
{{< /intro >}}

<div style="margin-top: 4rem;"></div>

Každý záznam v MemoMapě, který se má v mapě zobrazit, musí mít přiřazeno právě jedno takové místo. S místem vždy musíme vztahem propojit:

- adresu domu, kde někdo žil,  
- přesnou lokaci místa paměti (např. pamětní desky),  
- bod, kde došlo k incidentu,  
- polohu bodu zájmu (např. školy, synagogy nebo jiného objektu).

<div style="margin-top: 4rem;"></div>

## Jaké údaje o místech evidujeme

Struktura informací o místě obsahuje několik polí, která umožňují popsat adresu či lokalitu dostatečně přesně. Ne všechna pole musí být využita.


### 1. Základní charakteristika místa

- **Typ místa**  
  Jeden z předem definovaných typů, např.:  
  - dům
  - město
  - stát
  - místo věznění

- **Název**  
  Plná adresa místa tak, jak se zobrazí v MemoMapě (např. "Říčany, Masarykovo náměstí 7", "Pacov", "Terezín").  

### 2. Údaje o poloze (adresní struktura)

- **Město/obec**  
- **Ulice**  
- **Číslo domu**  

Obecně platí, že tato tři pole společně tvoří obsah pole **název**. Pokud se názvy ulic měnily, používá se zde původní (historický) název ulice.

### 3. Další názvy

Tabulka obsahuje také historické a současné popisy názvů, které mohou být užitečné u měst a obcí s bohatou historií:

- **Současný název** - současná varianta názvu místa, používáme stejný zápis jako v případě pole **Název**. 

Tento údaj není povinný. Využívá se tam, kde se názvy v čase měnily.

### 4. Poznámky

- **Poznámka**  
  Volný text pro interní informace, které se nezobrazují přímo uživateli, ale mohou pomoci při práci s adresami (např. „dům je dnes zbouraný“, „původní čp. 45 odpovídá dnešnímu čp. 102“).

### 5. Geografická poloha

- **Zeměpisné souřadnice**  
  Povinný atribut, bez kterého se místo nemůže zobrazit na mapě.  
  Obsahuje GPS bod (POINT) nebo jinou geometrii a určuje přesnou polohu.

V praxi se tyto souřadnice vybírají **kliknutím do mapy** nebo výběrem z existujícího seznamu adres. Tvůrce MemoMapy tedy nemusí zadávat souřadnice ručně.


<div style="margin-top: 4rem;"></div>

## Vztahy k dalším datovým typům v MemoMapě

**K místům se váže většina ostatních datových prvků MemoMapy.** Bez navázání na místa by aplikace nevěděla, kde jednitlivé body (např. místa paměti) zobrazit.

### 1. Vztah k osobám  
Každá osoba musí mít přiřazené minimálně jedno místo (např. poslední bydliště). Bez toho se nezobrazí v mapě.

### 2. Vztah k místům paměti  
Stolpersteine, pamětní desky a památníky mají vždy konkrétní fyzickou polohu, na které stojí/jsou položeny.

### 3. Vztah k bodům zájmu  
Synagogy, školy, hřbitovy či instituce jsou vázané na jedno konkrétní místo.

### 4. Vztah k incidentům  
Každý incident musí mít zadané právě jedno místo, kde se odehrál.

### 5. Vztah k událostem  
Současné události se odehrávají na konkrétním místě — před radnicí, v muzeu, před pamětní deskou.

### 6. Vztah k médiím  
U fotografií, dokumentů i jiných médií zachycujeme pomocí vztahu místo jejich vytvoření.

### 7. Vztah k příběhovým mapám  
Každá zastávka příběhové mapy má svůj bod nebo trajektorii (souslednou množinu bodů) na mapě.

<div style="margin-top: 4rem;"></div>

## Proč nejsou „místa“ samostatnou vrstvou?

Protože místo je **technická komponenta**, která umožňuje vykreslit na mapě ostatní datové typy.  

MemoMapa odděluje **obsah (osoby, body zájmu, incidenty, události, pamětní místa)** od **polohy (places)**. V praxi to výrazně zjednodušuje mapování i pozdější správu dat.

