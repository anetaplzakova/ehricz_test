# EHRI-CZ Hugo Site - Claude Context

## Projekt
Toto je **Hugo static site** pro **EHRI-CZ** (European Holocaust Research Infrastructure - Czech Node / Evropská infrastruktura pro výzkum holokaustu - český uzel).

## Základní informace
- **Framework**: Hugo (static site generator)
- **Hugo verze**: 0.111.3 nebo novější
- **Téma**: `ehri-nn` (ehri-nn-hugo-theme) - jako Git submodule v `themes/`
- **Jazyky**: Čeština (výchozí) + Angličtina
- **Účel**: Webová prezentace českého uzlu EHRI, výzkumné infrastruktury pro studium holokaustu

## Organizace
**Partnerské organizace**:
- Masarykův ústav a Archiv AV ČR
- Národní archiv
- Památník Terezín
- Institut Terezínské iniciativy

**Nadřazená infrastruktura**: LINDAT/CLARIAH-CZ (od 2023)

## Struktura projektu

### Konfigurace
- `config.yaml` - hlavní konfigurace (base URL, jazyky, menu, parametry)
- `defaultContentLanguage: cs`
- Kontakt: ehri@mua.cas.cz
- Sociální sítě: Facebook, Twitter/X, Bluesky

### Content (obsah)
`/content/` - Markdown soubory s obsahem stránek
- **Konvence názvů**: `nazev.cs.md` (čeština), `nazev.en.md` (angličtina)
- **Struktura front matter**: YAML blok mezi `---` a `---`
  ```yaml
  ---
  title: Titulek stránky
  description: Popis (volitelné)
  layout: about (volitelné)
  ---
  ```
- **Hlavní soubory**:
  - `_index.cs.md` / `_index.en.md` - úvodní stránka
  - `about.cs.md` / `about.en.md` - o projektu
  - `training.cs.md` / `training.en.md` - školení
  - `partners.cs.md` / `partners.en.md` - partneři
  - `news.cs.md` / `news.en.md` - aktuality
  - `/contact/` - kontakt
  - `/services/` - služby
  - `/news/` - jednotlivé novinky

### Data
`/data/` - YAML soubory s daty pro data-driven stránky
- **Konvence názvů**: `nazev.cs.yaml`, `nazev.en.yaml`
- **Soubory**:
  - `services.cs.yaml` / `services.en.yaml` - služby
  - `hlservices.cs.yaml` / `hlservices.en.yaml` - hlavní služby
  - `partners.cs.yaml` / `partners.en.yaml` - partneři
  - `people.cs.yaml` / `people.en.yaml` - lidé
  - `latest.cs.yaml` / `latest.en.yaml` - nejnovější aktuality
  - `hl-latest.cs.yaml` / `hl-latest.en.yaml` - hlavní aktuality

### Překlady
`/i18n/` - YAML soubory s překlady UI stringů
- `cs.yaml` - české řetězce
- `en.yaml` - anglické řetězce
- **Formát**:
  ```yaml
  key:
    other: "Překlad"
  ```

### Layouts & Assets
- `/layouts/` - Hugo šablony (HTML templates)
- `/assets/` - CSS, JS, obrázky pro zpracování
- `/static/` - statické soubory (kopírují se beze změny)
- `/themes/ehri-nn/` - téma jako Git submodule

## Hlavní služby EHRI-CZ
1. **MemoGIS** (https://ehri.cz/memogis/praha/)
2. **Holocaust.cz** (https://www.holocaust.cz/)
3. **Terezín Research Guide** (https://portal.ehri-project.eu/guides/terezin)
4. **EHRI Geodata** (https://geodata.ehri-project.eu/)

## Menu struktura
Definováno v `config.yaml`:
- **main** - hlavní menu (about, partners, news, services, contact)
- **footer** - patička (about, partners, news)
- **services** - submenu služeb (memogis, holocaustcz, terezin_research_guide, geodata)

Menu labels jsou v `/i18n/[lang].yaml`

## Běžné úkony

### Lokální development
```bash
hugo server
# Nebo s custom base URL:
hugo server --baseURL localhost:1313/test
```

### Build
```bash
hugo
# Výstup v /public/
```

### Update tématu
```bash
git submodule update --remote --merge
```

## Jak vytvořit novou stránku

1. Vytvoř nový soubor v `/content/` s příponou `.md`
2. Přidej front matter v YAML formátu:
   ```yaml
   ---
   title: Název stránky
   ---
   ```
3. Pokud je soubor pojmenován `nova-stranka.md`, bude dostupný na URL `/nova-stranka/`
4. **Pro vícejazyčný web**: vytvoř také `.en.md` verzi s přeloženým obsahem

### Vytvoření menu položky pro novou stránku

1. V `config.yaml` přidej nový záznam do `menu.main`:
   ```yaml
   menu:
     main:
       - identifier: nova_stranka
         pageRef: /nova-stranka/
         weight: 80
   ```
2. V `i18n/cs.yaml` a `i18n/en.yaml` přidej překlad:
   ```yaml
   nova_stranka:
     other: Nová stránka
   ```
3. Pro překlad EN menu přidej do `languages.en.menu.main`:
   ```yaml
   languages:
     en:
       menu:
         main:
           - identifier: nova_stranka
             pageRef: en/nova-stranka/
             weight: 80
   ```

## Důležité konvence

1. **Vždy vytvářej obsah v obou jazycích** (`.cs.md` + `.en.md`)
2. **Data soubory také duplikuj** (`.cs.yaml` + `.en.yaml`)
3. **Front matter je povinný** pro každý content soubor
4. **Menu identifiers** musí mít překlad v `i18n/[lang].yaml`
5. **Hugo shortcodes**: projekt používá např. `{{< intro >}}`, `{{< figure >}}`
6. **Unsafe HTML povoleno** (v `config.yaml` je `markup.goldmark.renderer.unsafe: true`)


## Shortcodes použité v projektu
- `{{< intro >}}...{{< /intro >}}` - intro sekce
- `{{< figure src="..." caption="..." class="..." >}}` - obrázky s popiskem

## Git
- **Main branch**: `main`
- **Submodules**: ano (téma v `/themes/ehri-nn/`)
- **Při klonování**: `git clone --recurse-submodules`

## Poznámky
- README.md je původní dokumentace z EHRI NN skeleton (pro Angličtinu + Velštinu)
- Projekt je adaptace pro češtinu + angličtinu
- Některé části jsou WIP (viz HTML komentáře v content souborech)