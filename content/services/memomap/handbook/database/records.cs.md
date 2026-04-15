---
title: Jak vytvářet a upravovat záznamy
layout: single
type: handbook
---

<div style="max-width: 53%">
  {{< figure src="../../images/directus-basics3.png" class="fig-float fig-left" >}}
</div>

{{< intro >}}

V této kapitole vysvětlíme, jak vytvářet a upravovat jednotlivé záznamy a jak pracovat s poli, která obsahují.

Každý záznam se skládá z několika typů polí – od jednoduchých textových údajů až po výběr z možností nebo zadání polohy v mapě. Správné vyplnění těchto polí je klíčové pro to, aby data fungovala jako celek.

{{< /intro >}}

<div style="margin-top: 4rem;"></div>

## Jak vytvořit nový záznam

Při vytváření nového záznamu postupujete jednoduše:

1. v levém menu vyberete typ dat (např. osoby, místa, incidenty),  
2. kliknete na tlačítko **+** v pravém horním rohu,  
3. otevře se formulář pro nový záznam,  
4. vyplníte jednotlivá pole,  
5. záznam uložíte pomocí tlačítka se symbolem fajfky v pravém horním rohu.  

K vytvořeným záznamům se můžete kdykoli vrátit a data doplňovat či upravovat.

<div style="display: flex; gap: 1rem; justify-content: space-between; margin-top: 1rem;">

  <div style="flex: 1; text-align: center;">
    <a href="../../images/directus-basics4.png">
      <img src="../../images/directus-basics4.png"
           alt="Directus"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>

  <div style="flex: 1; text-align: center;">
    <a href="../../images/directus-record1.png">
      <img src="../../images/directus-record1.png"
           alt="Directus"
           style="max-height: 220px; width: auto; display: block; margin: 0 auto;">
    </a>
  </div>
</div>

<div style="margin-top: 4rem;"></div>

## Jaké typy polí se v záznamech používají

Formuláře obsahují různé typy polí. Každé z nich má jinou funkci:

- **textová pole**  
  slouží pro zápis jmen, názvů nebo popisů,  

- **pole pro zadání data**  
  umožňují zadat konkrétní datum, např. datum narození, datum konání připomínkové akce apod.,

- **rozbalovací seznamy**  
  umožňují vybrat hodnotu z předem připraveného seznamu, např. typ místa paměti, osud dané osoby,  

- **pole pro vztahy**  
  slouží k propojení záznamu s jinými záznamy (např. osoba ↔ místo),  

- **pole pro přílohy**  
  umožňují připojit dokumenty či fotografie nebo jiná data,  

- **mapová pole**  
  slouží k určení polohy konkrétního bodu na mapě, relevantní pouze v případě míst.

Každé pole má v rámci formuláře své jasné místo a význam.

<div style="margin-top: 4rem;"></div>

## Specifická pole v záznamech

Pole jsou v záznamu vždy uvozena svým názvem, který je ve většině případů jasný a srozumitelně vysvětluje obsah pole. Specifická pole v některých záznamech, která si žádají bližší vysvětlení jsou:

- **ID záznamu**  
  jednoznačný identifikátor, který systém přiřadí automaticky, nemusíte jej doplňovat, 

- **typ** (tam, kde je relevantní)  
  pomáhá rozlišit konkrétní kategorii záznamu (např. typ místa nebo bodu zájmu),

- **status**  
  určuje stav záznamu, tedy zda je záznam rozpracovaný nebo hotový, indikuje, zda je třeba se k záznamu ještě vrátit.

<div style="margin-top: 4rem;"></div>
  
## Práce s místy a vztahy

Některé části práce se záznamy jsou důležitější a vyžadují podrobnější vysvětlení. Specifika práce s těmito záznamy vysvětlujeme v následujících kapitolách:

- <h5 style="margin-bottom: 0rem;">
  <a href="/services/memomap/handbook/database/records-places/">Jak pracovat s místy a polohou</a>
  </h4>

- <h5 style="margin-bottom: 0rem;">
  <a href="/services/memomap/handbook/database/records-relationships/">Jak propojovat data prostřednictvím vztahů</a>
  </h4>

<div style="margin-top: 4rem;"></div>

## Doporučení pro práci

- začněte základními údaji a postupně je doplňujte,  
- průběžně kontrolujte propojení mezi záznamy,  
- vždy dbejte na správné určení místa na mapě.  

Dobře vyplněný záznam je základní stavební kámen celé MemoMapy.