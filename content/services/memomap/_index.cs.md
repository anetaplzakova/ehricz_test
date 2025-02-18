---
title: MemoMapa | zkoumejte dějiny holokaustu v prostoru 
layout: training
type: training
date: 2024-09-09
---

{{< intro >}}
Projekt MemoMap umožňuje studovat historii holokaustu skrze prostor města a míst pronásledování. Název je odvozen z anglického memory map, tedy paměťová mapa, která propojuje informace o lidech, tedy historických aktérech, a místech, v nichž se pronásledování odehrávalo. Řadí se k dalším projektům, jež vkládají informace o historii holokaustu do mapy. MemoMapy usilují o využití velmi rozsáhlých souborů dat, mezi něž patří databáze obětí, digitalizovaných dokumentů z veřejných i soukromých archivů, historických map a dalších kontextuálních informací. V současnosti nabízíme MemoMapu pro město Praha a připravujeme k publikaci obdobnou aplikaci pro město Pacov. Doufáme, že v dalších letech přidáme další místa a nové funkce. 
{{< /intro >}}

<br/>

[Vstup do aplikace zde.](http://www.memomap.cz)

[Více o MemoMap Praha naleznete zde.](/services/memomap/prague/)

{{< figure src="/images/memomap.png" class="fig-float fig-right" >}}

<br/>

### MemoMapy a konstrukce prostoru

Při práci na MemoMapách se inspirujeme výzkumem o geografických informačních systémech (GIS) a poznatky z různých oblastí geografie a kartografie. Mezi ty patří též kritické přístupy vycházející ze sociální konstrukce prostoru: dnes víme, že není daný jen koordináty a měřitelnými vzdálenostmi, ale je tvořen každodenním setkáváním lidí, jejich jednáním a představami. Mapy a další prostorové politiky jsou také nástroji moci a mohou vytvářet společenské hierarchie: v tomto případě vylučování a pronásledování skupiny lidí označených za rasově odlišné. 

Jsme si také vědomi toho, že ne všechno lze vyjádřit v geografických koordinátech a zobrazit na běžné mapě prostřednictvím bodů, čar či jiných geometrických tvarů. Týká se to například emocí lidí vztahujících se k prostoru, ale také událostí, jejichž přesné místo není známé. I proto přístupy přicházející z geografických informačních systémů doplňujeme o historické dokumenty a další informace, přemýšlíme o spojení s narativy obětí a dalšími formami interaktivní prezentace negeometrických dat. 

Konstrukce prostoru není jen historickým fenoménem: MemoMapy samy jsou také vědomou intervencí v současném veřejném prostoru a příspívají k tomu, aby badatelé přemýšleli o mechanismech sociální inkluze a exkluze v každodenním životě. Používání aplikace ovlivňuje nejen znalosti uživatelů, ale také jejich vnímání míst a prostoru. Za tímto účelem a nad rámec toho, co nabízí řada podobných aplikací, klade projekt zvláštní důraz na data, která obohacují prostorovou zkušenost, a na povědomí o sdíleném prostoru.

### Kdo může MemoMapy používat? 

Kdokoli. MemoMapy staví na principu, že badatelem se může stát každý, a jsou otevřené pro vědecké i laické využití. Aplikace je přizpůsobena zobrazení na mobilních zařízeních a uživatelé se s ním mohou vydat přímo do prostoru města či míst paměti. 

Vědcům umožňují formulovat nové otázky o dějinách holokaustu, například o procesu vylučování ze společnosti, prostorové segregaci či formách vzdoru ze strany pronásledovaných, využívat statistické údaje a přímo též pracovat s většinou datových sad, jež MemoMapy zpřístupňují, a to zejména prostřednictvím EHRI Repozitoře pro geoprostorová data (viz níže).  

Obyvatelům i studentům pomáhají zkoumat historii holokaustu přímo v místech, kde žijí, pracují nebo kde se běžně pohybují. Rodinám obětí doplní již známé informace publikované v Terezínských pamětních knihách a databázi obětí na serveru www.holocaust.cz o umístění do prostoru města. 

Aplikaci lze také využít jako vzdělávací nástroj pro výuku o lidských právech, holokaustu nebo dějinách rasismu a antisemitismu. Podporuje moderní přístup k vúuce dějepisu a dalších předmětů založenou na samostatném bádání studentů a interaktivní práci ve veřejném prostoru. Zahrnutím osobních příběhů, fotografií a dokumentů doplňuje výuku o „velkých dějinách“ mikrohistorickými metodami. 

Turistům umožňuje jiný způsob zkoumání navštívených míst a zároveň významným způsobem rozšiřuje existující muzejní expozice a památníky.

### Technické řešení

Implementace uživatelského rozhraní MemoMapy vychází ze zkušenosti získané na základě testovací mobilní aplikace a provizorního webového rozhraní k serveru QGIS. Úplně nový softwarový základ nám umožňuje snazší úpravy uživatelského rozhraní, zahrnutí časové osy a fulltextové vyhledávání ve jménech a adresách. 

Nová memomapa je od začátku přizpůsobena pro mobilní zobrazení. Její kód je založený na na opensource knihovnách a nástrojích (ASP.NET Core, Blazor WASM). Uživatelé mohou tuto responzivní webovou aplikaci spustit ve webových prohlížečích na počítači a na operačních systémech Android a iOS. Vzhledem k velkému počtu záznamů a dokumentů a jejich průběžné aktualizaci vyžaduje aplikace stálé připojení k internetu.  

Projekt podporuje co největší otevřenost a duplikovatelnost. Kód aplikace je volně přístupný prostřednictvím sotwarové repozitoře Github a je možné jej dále rozvíjet v rámci dalších projektů. 

S výjimkou informací podléhajících ochraně osobních dat jsou data použítá v MemoMapách přístupná také prostřednictvím EHRI Repozitoře geoprostorových dat (EHRI Geospatial Repository). Je možné s nimi proto pracovat v libovolném GIS software a jiným způsobem.

### O projektu

Aplikaci MemoMap vytvořil Masarykův ústav a archiv Akademie věd ČR jako službu českého uzlu Evropské infrastruktury pro výzkum holokaustu (EHRI). Ten je součástí infrastruktury LINDAT/CLARIAH-CZ, která je plně podporována Ministerstvem školství, mládeže a tělovýchovy České republiky v rámci programu „velkých infrastruktur“. Příprava dat a vytvoření nového softwaru bylo dále možné díky podpoře Nadačního fondu obětem holokaustu a programu Strategie AV21 Město jako laboratoř změny. 

Navazuje na aplikaci MemoGIS Praha, jež byla výsledkem projektu Integrace a segregace v prostoru města: dějiny holokaustu v Praze prostřednictvím mobilní webové aplikace (idenifikátor TL01000366). Ten byl podpořen Technologickou agenturou České republiky v rámci veřejné soutěže ÉTA 1 a na původní aplikaci MemoGIS spolupracoval Masarykův ústav a archiv AV ČR s Institutem Terezínské iniciativy a Multikulturním centrem Praha. 
