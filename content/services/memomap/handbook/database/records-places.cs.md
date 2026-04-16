---
title: Jak pracovat s místy a polohou
layout: single
type: handbook
---

<div style="max-width: 75%;">
  {{< figure src="../../images/directus-records-places1.png" class="fig-float fig-left" >}}
</div>

{{< intro >}}

Při práci se záznamy v editačním rozhraní se velmi často setkáte s polem pro **výběr nebo vytvoření vztahujícího se místa**.

U většiny typů dat (např. osoby, incidenty nebo pamětní místa) je přiřazení vztahu k místu nezbytné – bez něj se záznam v mapě nezobrazí.

Přiřazení vztahu k místu probíhá ve formulářích jednotlivých datových typů (osoby, incidenty apod.), ale je možné pouze v případě, že takové místo předem existuje v seznamu míst. Pokud místo zatím v seznamu míst chybí, je třeba jej nejprve vytvořit a přidat k němu zeměpisné koordináty, které určují polohu místa v mapě.

{{< /intro >}}

<div style="margin-top: 4rem;"></div>

## Jak s místy pracovat

Základní seznam míst bude ve vašem projektu částečně **předpřipravený** a bude obsahovat místa, která se v datech často opakují. Místa specifická pro vaši MemoMapu, např. konkrétní adresy ve vašem městě, však bude nutné do seznamu míst nejprve doplnit.

**Platí, že:**

- konkrétní adresy a lokality ve vašem městě budete ve většině případů **vytvářet sami**,  
- nová místa zakládáte stejným způsobem jako jiné záznamy (pomocí tlačítka **+**),  
- jednotlivá pole vyplňujete stejně jako u jiných typů dat.  

Specifickým prvkem u míst je pole pro **určení polohy daného místa na mapě**.

<div style="margin-top: 4rem;"></div>

## Jak zadat polohu na mapě

Polohu místa zadáváte pomocí mapového pole, které je součástí formuláře.

**Postup:**

- vyhledejte požadované místo v mapě pomocí přiblížení a posouvání mapy (přiblížení a oddálení je možné pomocí tlačítek v okně mapy vlevo nebo jednoduše kolečkem myši),
- v menu na levé straně okna s mapou vyberte tlačítko "Marker tool", které vám do mapy umožní přidat bod,
- klikněte na konkrétní místo na mapě a přidejte bod,  
- polohu bodu můžete případně dále upravovat jeho posunutím, rovněž jej můžete smazat pomocí tlačítka koše na levé straně okna s mapou a začít znovu,  
- uložte záznam.

Systém automaticky uloží zeměpisné koordináty (souřadnice) zvoleného bodu.

<div style="display: flex; gap: 1rem; justify-content: space-between; margin-top: 1rem;">

  <div style="flex: 1; text-align: center;">
    <a href="../../images/directus-records-places2.png">
      <img src="../../images/directus-records-places2.png"
           alt="Vyhledání místa"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 1; text-align: center;">
    <a href="../../images/directus-records-places3.png">
      <img src="../../images/directus-records-places3.png"
           alt="Kliknutí do mapy"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 1; text-align: center;">
    <a href="../../images/directus-records-places4.png">
      <img src="../../images/directus-records-places4.png"
           alt="Úprava polohy"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

</div>


<div style="margin-top: 3rem;"></div>

### Na co si dát pozor

- u přesných adres se snažte umístit bod co nejpřesněji (např. na konkrétní dům či místo ve městě),  
- u historických míst, která dnes neexistují, určete polohu co nejpřesněji podle dostupných podkladů,  
- pokud si nejste jistí, je lepší zvolit přibližnou polohu než pole nechat prázdné.  

<div style="margin-top: 4rem;"></div>

