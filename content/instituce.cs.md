---
title: "EHRI pro paměťové instituce: Začleňte svá data do portálu EHRI"
aliases:
  - /pro-pametove-instituce/
---

![Sdílení metadat sbírek s EHRI](/images/EHRI-for-Institutions-CZ.jpg)

Informace o pramenech vztahujících se k tématu holokaustu jsou nezbytné pro výzkum, vzdělávání i připomínání. **Uchováváte takové prameny vy nebo vaše instituce a chcete, aby informace o nich byly viditelné a snadno dohledatelné?** Přečtěte si, jak lze tyto informace zpřístupnit prostřednictvím Portálu EHRI.

## Proč EHRI?

[Portál EHRI](https://portal.ehri-project.eu/) poskytuje přístup k informacím o archivních materiálech vztahujících se k holokaustu, které jsou uloženy v institucích po celé Evropě i mimo ni, a zároveň tato data vzájemně propojuje. Začleněním popisů archivních materiálů do portálu EHRI zvýšíte mezinárodní viditelnost své instituce, zlepšíte dohledatelnost svých dat i instituce samotné, zajistíte, aby data splňovala principy [FAIR](https://www.nature.com/articles/sdata201618) (Findable, Accessible, Interoperable, Reusable – dohledatelná, přístupná, interoperabilní a opakovaně využitelná), a stanete se součástí sítě institucí a odborníků, s nimiž můžete sdílet zkušenosti i odborné znalosti. Vaše data zůstávají i po zařazení do Portálu EHRI plně pod vaší kontrolou.

Krátké úvodní video představující Portál EHRI naleznete [zde](https://www.youtube.com/watch?v=IUFqR7l5qW8).

Pro uživatele je zásadní, aby věděli, kde jsou archivní materiály uloženy a zda jsou přístupné ke studiu. Proto si nejprve ověřte, zda je vaše instituce – případně vy jako soukromá osoba – již zaregistrována v Portálu EHRI. Pokud tomu tak není, kontaktujte nás prosím na adrese [archives@ehri-project.eu](mailto:archives@ehri-project.eu) s předmětem „new input for the EHRI Portal“ (nový příspěvek do Portálu EHRI) a uveďte, kterou instituci si přejete do Portálu EHRI přidat.

## Jaká (meta)data Portál EHRI podporuje?

Portál EHRI poskytuje přístup k archivním popisům materiálů vztahujících se k tématu holokaustu, označovaným také jako archivní pomůcky (finding aids) nebo seznamy fondů a sbírek (holdings lists). Archivní popisy poskytují badatelům informace o struktuře archivních materiálů, jejich formátu, obsahu i možnostech přístupu.

Samotné archivní materiály ani jejich případné digitální reprodukce nejsou v Portálu EHRI uloženy a zůstávají plně ve správě instituce, která je uchovává. Jinými slovy, Portál EHRI zpřístupňuje metadata (popisy archivních materiálů), nikoli samotná data (archivní materiály).

## Výběr relevantních materiálů

Zvažte, zda se všechny popisy fondů a sbírek ve vaší instituci vztahují k holokaustu. Pokud ne, můžete pro zpřístupnění v rámci Portálu EHRI vybrat pouze ty, které s holokaustem souvisejí. Potřebujete-li s výběrem poradit, neváhejte kontaktovat tým EHRI.

## Jak mohu zařadit své archivní popisy do Portálu EHRI?

Archivní popisy fondů a sbírek lze v Portálu EHRI zpřístupnit několika způsoby. Jednotlivé možnosti se liší mírou technické náročnosti:

![Sdílení metadat sbírek s EHRI](/images/EHRI-for-Institutions-CZ.jpg)

| Způsob | Popis |
| --- | --- |
| **Ruční zadávání dat** | Popisy fondů a sbírek zadáváte sami přímo do Portálu EHRI prostřednictvím uživatelského účtu určeného pro správu obsahu. |
| **Hromadný import** | EHRI importuje popisy vašich fondů a sbírek ze souborů XML, nejlépe ve standardizovaném formátu Encoded Archival Description (EAD). |
| **Opakovatelné hromadné importy** | EHRI automaticky stahuje metadata vašich fondů a sbírek z veřejně dostupného webového umístění a pravidelně je importuje do Portálu EHRI. Tento proces se v nastavených intervalech opakuje, aby popisy v Portálu zůstávaly aktuální. |

## Další kroky

Budete-li mít během tohoto procesu jakékoli dotazy, neváhejte kontaktovat tým EHRI na adrese [archives@ehri-project.eu](mailto:archives@ehri-project.eu).

## Často kladené otázky (FAQ)

### Jaký datový formát EHRI používá pro hromadný import?

Pro import archivních popisů do Portálu EHRI používáme formát [EAD 2002](https://en.wikipedia.org/wiki/Encoded_Archival_Description). Kromě toho, že data musí být validní podle schématu EAD, je nutné, aby každá archivní jednotka (v EAD část označená elementem `<did>`) obsahovala identifikátor `<unitid>`, který je jedinečný v rámci sourozeneckých jednotek na stejné úrovni hierarchie. Tento požadavek sice není součástí standardu EAD, je však nezbytný pro jednoznačnou identifikaci zdroje dat pro účely zařazení do Portálu EHRI. Ideální je, pokud je každý `<unitid>` jedinečný v rámci celé instituce, není to však nezbytnou podmínkou.

Před samotným importem EHRI data normalizuje a odstraňuje některé méně používané prvky formátu EAD, zejména ty, které se týkají formátování textu, a prvky, které Portál EHRI dosud nepodporuje.

### Co když nemohu poskytnout data ve formátu EAD?

Ne všechny systémy podporují export do formátu EAD. Pokud však data splňují konkrétní strukturální požadavky (například jeden soubor obsahuje popis pouze jednoho archivního fondu nebo sbírky), lze je před importem převést do formátu EAD s využitím nástrojů EHRI.

S technickými požadavky vám rádi poradí odborníci z EHRI Mobile Lab.

Pokud jsou data uložena v jiném než XML formátu, například ve formátu CSV nebo Microsoft Excel, může být nutné připravit převod dat individuálně.

### Podporujete také EAD-3?

Ano. Přestože formát EAD-3 dosud neprošel tak rozsáhlým testováním jako EAD 2002, Portál EHRI podporuje import i této nejnovější verze standardu.

### Podporujete vícejazyčné archivní pomůcky?

Ano. Prostřednictvím formátu EAD lze importovat vícejazyčné archivní pomůcky, pokud je každá jazyková verze uložena v samostatném XML souboru. Vícejazyčné funkce standardu EAD-3 však Portál EHRI *zatím* nepodporuje.
