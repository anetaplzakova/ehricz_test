---
title: Jak funguje uživatelské rozhraní
layout: single
type: handbook
---

<div style="max-width: 53%;">
  {{< figure src="../../images/directus-basics.png" class="fig-float fig-left" >}}
</div>

{{< intro >}}

Pro práci s daty používáme nástroj **Directus**, který slouží jako přehledné uživatelské rozhraní nad databází.

Pro vás to znamená, že nemusíte řešit technickou stránku projektu – všechny údaje zadáváte prostřednictvím jednoduchých formulářů. Každý formulář odpovídá určitému typu dat (např. osoba, místo nebo událost) a umožňuje vám data snadno vytvářet, upravovat a propojovat.

{{< /intro >}}

<div style="margin-top: 4rem;"></div>

## Jak je rozhraní uspořádané

<div style="max-width: 100%;">
	<a href="../../images/directus-basics2.png">
  {{< figure src="../../images/directus-basics2.png" class="fig-float fig-right" >}}
	</a>
</div>

Uživatelské rozhraní se skládá z několika základních částí:

- **levé menu** – obsahuje záložky jednotlivých typů dat, s nimiž v rámci svého projektu pracujete (např. lidé, místa, incidenty),  
- **seznam záznamů** – přehled všech položek daného typu (např. všech osob), který se zobrazí po výběru typ dat v levém menu, 
- **detailní záznam** – formulář, ve kterém vyplňujete detailní údaje o osobách, místech ad.  

Každý typ dat má vlastní formulář, ale princip práce s nimi je vždy stejný.

<div style="margin-top: 4rem;"></div>

## Záznam jako základní jednotka

<div style="max-width: 100%">
	<a href="../../images/directus-basics3.png">
  {{< figure src="../../images/directus-basics3.png" class="fig-float fig-right" >}}
	</a>
</div>

Vždy platí, že:

- jedna osoba = jeden záznam,  
- jedno místo = jeden záznam,  
- jedna událost = jeden záznam.  

Každý záznam obsahuje předdefinovaná pole, která odpovídají typu informace, s níž pracujete (např. pole datum narození je relevantní pro osoby, ale nikoli pro místa).

<div style="margin-top: 4rem;"></div>

## Jak zadáváte data

<div style="max-width: 100%">
	<a href="../../images/directus-basics4.png">
  {{< figure src="../../images/directus-basics4.png" class="fig-float fig-right" >}}
	</a>
</div>

Při práci postupujete jednoduše:

1. vyberete typ dat v levém menu,  
2. vytvoříte nový záznam pomocí tlačítka "+" vpravo nahoře,  
3. vyplníte dostupné údaje,  
4. záznam uložíte.  

Vytvořený záznam můžete kdykoli znovu otevřít a upravit. Jednoduše jej vyberete ze seznamu záznamů.

<div style="margin-top: 4rem;"></div>

## Ne všechna pole je nutné vyplnit

- některá pole jsou **povinná** (označena hvězdičkou),  
- většina polí je **nepovinná**.  

Je v pořádku pracovat i s neúplnými daty – informace můžete postupně doplňovat.

<div style="margin-top: 4rem;"></div>

## Propojení dat je klíčové

Jednotlivé záznamy mezi sebou vytvářejí vztahy, které jsou důležité pro jejich správné zobrazení v mapě.

Například:

- osoba je propojená s místem, kde žila, nebo s další osobou (rodinné vztahy)  
- dokument je propojený s osobou nebo bodem zájmu, který zachycuje,  
- incident je propojený s konkrétní osobou nebo událostí.  

Bez těchto vazeb by data zůstala izolovaná a v mapě by nedávala smysl. Pole pro zadání vztahů je vždy součástí formuláře záznamu.

<div style="margin-top: 4rem;"></div>