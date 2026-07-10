---
name: add-news
description: Přidání nové vícejazyčné novinky (Hugo) a aktualizace souborů s odkazy. Argumentem musí být název souboru (např. 'novinka.md').
---

# Přidání nové vícejazyčné novinky

Tento skill slouží k přidání nové vícejazyčné novinky pro Hugo statický generátor stránek a aktualizaci souborů s odkazy.

## Instrukce pro provedení úkolu
Při spuštění tohoto skillu proveďte následující kroky:

1. Vytvoř nový adresář pro novinku v cestě: `content/news/`
2. Vytvoř v tomto novém adresáři soubory s obsahem v češtině a angličtině (zahrň i potřebné front matter/metadata pro Hugo).
3. Vlož krátký výtah z novinky (titulek a krátký popis/úvodní text) do následujících souborů s odkazy na novinky:
   - `data/hl-latest.cs.yaml`
   - `data/hl-latest.en.yaml`
   - `data/latest.cs.yaml`
   - `data/latest.en.yaml`
4. Pozor, odkaz-url na anglickou verzi novinek musí vždy začínat `/en/...`, tedy například `/en/news/novinka/`; odkazy na českou verzi novinek nemusí obsahovat kód pro jazyk, stačí tedy `/news/novinka/`.
5. Vstupní data (formát: `soubor.md -- dodatečné instrukce`) jsou předány jako argumenty.

### DŮLEŽITÉ
- První část vstupu (před `--`) považuj za název souboru.
- Druhou část vstupu (za `--`) považuj za dodatečné instrukce. Pokud druhá část chybí, instrukce ignoruj.
