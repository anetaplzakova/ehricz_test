---
title: Typy dat v MemoMapě
layout: single
type: handbook
---

{{< intro >}}
Při tvorbě MemoMapy pracujeme s různými typy informací, které se pak v aplikaci zobrazují různými způsoby. Některé z nich představují tzv. **vrstvy mapy**, které si uživatel může v mapě prohlížet. Jiné představují tzv. **podpůrná data**, která se v mapě nezobrazují samostatně, ale jsou zásadní z hlediska propojení údajů a mapy, propojování jednotlivých typů dat mezi sebou a také nesou důležité kontextové informace.

Aby byla práce na MemoMapě srozumitelná a přehledná, data v této části příručky dělíme do několika skupin podle jejich účelu. S každou skupinou dat při tvorbě MemoMapy pracujeme trochu jiným způsobem. Na této stránce najdete stručný přehled toho, co která kategorie obsahuje a jak se zobrazuje ve výsledné mapě.
{{< /intro >}}

<div style="margin-top: 4rem;"></div>

## 1. Data, která tvoří základ mapy (hlavní vrstvy)

Tyto typy dat odpovídají **vrstvám přímo viditelným v aplikaci**. Uživatel si je může zapínat a vypínat podle toho, co právě sleduje. Například může zobrazit jen místa paměti, jen body zájmu nebo jen incidenty a vybrat si, zda je chce zobrazit na současné nebo historické mapě města/obce. Patří sem:

- **[Osoby](/services/memomap/handbook/datatypes/entities/)** – jádro MemoMapy, data a příběhy místních židovských obyvatel, v mapě se sdružují do jednotlivých domů (bydlišť osob), které tvoří rozcestník k jednotlivým osobám a jejich osudům
- **[Body zájmu](/services/memomap/handbook/datatypes/points-of-interest/)** – synagogy, školy a jiná zajímavá místa spojená s životem místní židovské komunity  
- **[Místa paměti](/services/memomap/handbook/datatypes/places-of-memory/)** – místa připomínání, například kameny zmizelých (Stolpersteine), pamětní desky nebo jiné památníky  
- **[Incidenty](/services/memomap/handbook/datatypes/incidents/)** – historické události spojené s perzekucí židovských obyvatel obce, například na místech, kde byl někdo zatčen 
- **[Události](/services/memomap/handbook/datatypes/events/)** – současné pipomínkové akce, výstavy a jiné události spojené s připomínkou obětí holokaustu
- **[Historická mapa](/services/memomap/handbook/datatypes/historical-map/)** – mapový podklad, který ukazuje, jak město vypadalo v určité době

Kromě historické mapy, která se zpracovává zvláštním způsobem, jsou všechny typy dat uloženy v jednoduché databázi, se kterou jako tvůrce obsahu MemoMapy budete pracovat. Pro každý typ informací se doplňuje několik základních údajů, které se poté zobrazí na mapě.

### Jak MemoMapa pracuje s místy a polohou:

Všechny výše uvedené datové typy se v mapě zobrazují **na určitém místě** – u konkrétního domu, na ulici nebo jinde v prostoru města/obce (park, most nábřeží apod.).

**[Místa](/services/memomap/handbook/datatypes/places/)** proto **nejsou samostatná datová vrstva**, ale technický prvek, který:

- propojuje jednotlivé datové typy (obsahové záznamy) s konkrétní polohou  (například památník obětem holokaustu s průčelím parku, ve kterém stojí),
- zajišťuje, že se v mapě zobrazí na správném místě,  
- umožňuje jednotně pracovat s adresami a mapovými souřadnicemi.

<div style="margin-top: 4rem;"></div>

## 2. Kontextová a doplňující data

Některé informace mapě nezobrazují jako samostatné vrstvy, k jednotlivým hlavním datovým typům ale **přidávají důležité doplňkové informace** a kontext. Patří sem:

- **[Dokumenty, fotografie a další média](/services/memomap/handbook/datatypes/media/)** – obohacují detail osoby, místa paměti nebo ostatních prvků na mapě (uživatel pak v aplikaci vidí například fotografii konkrétní osoby, historický úřední dokument, nebo třeba video z připomínkové akce),  
- **[Příběhové mapy](/services/memomap/handbook/datatypes/story-maps/)** – nejsou samostatnou vrstvou jednotlivých značek, ale **nadstavbou** nad osobami či body zájmu, představují propojenou řadu zastávek, které společně do detailu vyprávějí příběh (například příběh jednoho z obyvatel města)

<div style="margin-top: 4rem;"></div>

## Proč má MemoMapa tolik složek?

Na první pohled to působí, že typů dat je hodně. Každý z nich má ale při tvorbě mapy své místo:

- některé vyprávějí **příběhy lidí a prostoru, ve kterém tito lidé žili** (osoby),  
- některé zachycují **způsob, jakým si události holokaustu vaše město/obec připomíná** (místa paměti, události),  
- jiné rekonstruují **konkrétní historické události** (incidenty),  
- další přidávají **doprovodný vizuální materiál** (fotografie, dokumenty),  
- a jiné umožňují detailní **vyprávění** konkrétního příběhu (příběhové mapy).

Dohromady vytvářejí obraz, který by žádný typ dat sám o sobě nedokázal postihnout.

Každá MemoMapa je jiná a informace, které má její tvůrce k dispozici, se vždy liší. Žádná z hlavních vrstev MemoMapy není "povinná" a při tvorbě mapy pracujeme vždy s informacemi, které jsou pro danou obec důležité a dostupné.

Může se také stát, že žádná z datových vrstev nepostihuje informace, které máte k dispozici a chcete zveřejnit vy. V tom případě nalezneme vhodné řešení společně – individuálně probereme vaše potřeby a strukturu mapy jim vhodně přizpůsobíme.

