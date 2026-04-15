---
title: Jak propojovat data prostřednictvím vztahů
layout: single
type: handbook
---

<div style="max-width: 95%;">
  {{< figure src="../../images/directus-records-relationships1.png" class="fig-float fig-left" >}}
</div>

{{< intro >}}

Při práci s daty v MemoMapě spolu jednotlivé záznamy **propojujete pomocí vztahů**.

Vztahy určují, jak spolu jednotlivé záznamy souvisejí – například která osoba žila na konkrétním místě, který dokument se k ní vztahuje nebo jaké osoby patří do jedné rodiny.

Díky vztahům se jednotlivé informace propojují do smysluplných celků a mohou být správně zobrazeny v mapové aplikaci MemoMap.

{{< /intro >}}


<div style="margin-top: 4rem;"></div>


## Co je vztah a jaké typy vztahů existují

Vztah je propojení mezi dvěma záznamy, například:

- osoba může být propojena s místem (narození, úmrtí, bydliště ad.),  
- osoba může být propojena s další osobou (rodinné vztahy),  
- dokument může být propojen s osobou, bodem zájmu apod.,  
- incident může být propojen s konkrétní osobou i místem. 

Podrobný přehled vztahů pro jednotlivé typy dat jsme podrobně popsali v kapitole **[Typy dat v MemoMapě](/services/memomap/handbook/datatypes/)**.

Pole pro zadání vztahů k ostatním záznamům jsou vždy součástí příslušného formuláře záznamu (např. pole pro zadání příbuzenského vztahu v záznamu osoby ad.).

<div style="margin-top: 4rem;"></div>


## Jak přidat vztah mezi záznamy

Vztahy přidáváte přímo ve formuláři záznamu pomocí pole pro výběr souvisejících položek.

**Postup:**

- v poli příslušného vztahu klikněte na tlačítko **„Přidat existující“**,
- kliknutí otevře seznam položek v pravé části obrazovky,  
- zaškrtnětě příslušnou položku a vztah vložte do záznamu kliknutím na tlačítko v prvé horní části nad seznamem,  
- pozor, vztah se do záznamu neuloží, dokud záznam neuložíte (tlačítko pro uložení v pravém horním rohu záznamu). 

Tímto způsobem vytvoříte základní vztah mezi dvěma záznamy.

<div style="display: flex; gap: 1rem; justify-content: space-between; margin-top: 1rem;">

  <div style="flex: 1; text-align: center;">
    <a href="../../images/directus-records-relationships2.png">
      <img src="../../images/directus-records-relationships2.png"
           alt="Výběr záznamu"
           style="max-height: 220px; width: 100%; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 1; text-align: center;">
    <a href="../../images/directus-records-relationships3.png">
      <img src="../../images/directus-records-relationships3.png"
           alt="Přidání vztahu"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 1; text-align: center;">
    <a href="../../images/directus-records-relationships4.png">
      <img src="../../images/directus-records-relationships4.png"
           alt="Přidání vztahu"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>
  
</div>

<div style="margin-top: 4rem;"></div>

## Vztahy s doplňujícími údaji

V některých případech nestačí pouze propojit dva záznamy – je potřeba doplnit i **další informace o samotném vztahu**. Bez tohoto upřesnění bychom nevěděli, co daný vztah znamená.

Typicky jde například o:

- určení typu vztahu mezi osobami (např. rodič, sourozenec),  
- určení typu vztahu mezi osobou a místem (např. místo narození, poslední bydliště před deportací),  
- nebo doplnění časového rozsahu (např. od kdy do kdy daný člověk bydlel na dané adrese).  

Pokud je upřesnění vztahu vyžadováno, systém vás nenechá záznam bez doplnění těchto údajů uložit.

<div style="margin-top: 2rem;"></div>



### Jak doplňující údaje o vztahu vložit?

Způsob vytvoření vztahu se nemění, probíhá stejně jako u jednoduchých vztahů (výběr ze seznamu a uložení, viz výše). Doplňující údaje o vztahu přidáte v následujícím kroku:

- kliknete do pole právě vytvořeného vztahu (pozor, dokud záznam neuložíte, vztah se do formuláře nepropíše a nově doplněný vztah tedy vidíte pouze jako dvě čárky „--“),  
- kliknutí otevře formulář v pravé části obrazovky, do nějž doplníte požadované informace vztahu,  
- informace o vztahu uložíte.

<div style="display: flex; gap: 1rem; justify-content: space-between; margin-top: 1rem;">

  <div style="flex: 1; text-align: center;">
    <a href="../../images/directus-records-relationships5.png">
      <img src="../../images/directus-records-relationships5.png"
           alt="Výběr záznamu"
           style="max-height: 220px; width: 100%; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 1; text-align: center;">
    <a href="../../images/directus-records-relationships6.png">
      <img src="../../images/directus-records-relationships6.png"
           alt="Přidání vztahu"
           style="max-height: 220px; width: 100%; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 1; text-align: center;">
    <a href="../../images/directus-records-relationships7.png">
      <img src="../../images/directus-records-relationships7.png"
           alt="Přidání vztahu"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>
  
</div>
