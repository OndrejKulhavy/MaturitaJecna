
<div align="center">
  <img src="https://www.spsejecna.cz/ci/SPSE-Jecna_Logotyp.png" alt="SPSE Jecna Logotyp" width="400" style="margin: 20px;">
</div>

# Maturitní Téma: Metodiky a životní cyklus vývoje softwaru

- **Anki Flashcards**: [![Anki Flashcards](https://img.shields.io/badge/Anki-Flashcards-1f425f.svg)](https://ankiweb.net/shared/info/)
- **Autoři**: @danielkahoun @MaksymDoremi @OndrejKulhavy

# Shrnutí

Tento text se zabývá metodikami a životním cyklem vývoje softwaru, konkrétně Software Development Life Cycle (SDLC). Obsahuje analýzu a plánování, návrh, implementaci, testování, nasazení a údržbu. Dále porovnává různé metodiky vývoje, jako je Waterfall, Spirální model, Agilní přístup (s důrazem na Scrum), Extrémní programování, Prototypovací model a RUP (Rational Unified Process).

Text zdůrazňuje, že SDLC slouží jako rámec pro plánování, návrh a údržbu softwarových systémů, s každou fází zaměřenou na specifické cíle. Porovnání metodik ukazuje, že Agilní přístup a Scrum nabízejí rychlou zpětnou vazbu a flexibilitu, ale vyžadují úzkou spolupráci se zákazníkem. Spirální model kombinuje designový a prototypový přístup, zatímco RUP nabízí iterativní a inkrementální přístup vhodný pro velké projekty.

Text rovněž prezentuje výhody a nevýhody jednotlivých metodik, například jednoduchost Waterfallu a jeho nepružnost vůči změnám, flexibilitu Spirálního modelu na úkor nákladů a časové náročnosti, a agilní přístup s jeho rychlým dodáním, ale náročným plánováním. RUP zdůrazňuje důkladnou dokumentaci a schopnost odhalit chyby, ale může být nákladný a nevhodný pro malé projekty.
## Video
Odkaz na případné video, které ilustruje nebo doplňuje téma

# Obsah
- [Shrnutí](#shrnutí)
- [Video](#video)
- [Obsah](#obsah)


- [Metodiky a životní cyklus vývoje softwaru](#metodiky-a-životní-cyklus-vývoje-softwaru)
- [Často používané fáze v rámci životního vývoje softwaru (SDLC)](#často-používané-fáze-v-rámci-životního-vývoje-softwaru-sdlc)


- [Waterfall](#waterfall)
- [Spirální model](#spirální-model)
- [Agilní přístup](#agilní-přístup)
  - [Scrum](#scrum)
  - [Extrémní programování (XP)](#extrémní-programování-xp)
  - [Prototypovací model](#prototypovací-model)
  - [RUP (Rational Unified Process)](#rup-rational-unified-process)

--- 

# Metodiky a životní cyklus vývoje softwaru
SDLC (Software Development Life Cycle) je soubor procesů nebo fází, které softwarový produkt prochází od jeho návrhu až po jeho údržbu a odstranění z provozu. SDLC je rámec, který organizace používají k plánování, návrhu, vytváření, testování a údržbě softwarových systémů. Každá fáze SDLC má své vlastní cíle a úkoly, a celkově pomáhá zajistit, že vývoj softwaru probíhá systematicky a efektivně.

## Často používané fáze v rámci životního vývoje softwaru (SDLC)
Fáze popsané níže se mírně liší na základě vybrané metodiky vývoje. V základu jsou ale všechy stejné.

### Analýza a plánování
- Identifikace problémů k řešení
- Požadavky
- Definování cílů

### Návrh
- Na základě požadavků zákazníka se vytvoří návrh na technické řešení
- Zpracování analýzy - UML diagramy, logické a relační schéma databáze
- Volba frameworků, programovacích jazyků, vývojového prostředí, CDN (cloudy, provozovny) apod.
- Odhad ceny
  - za celou zakázku - Waterfall..
  - za iteraci - agilní metodiky (např. Scrum)

### Implementace
- Samotná tvorba zdrojového kódu / databáze
- Optimalizace

### Testování
- Quality assurance tým naplní demo verzi prvními testovacími daty.
- Ověří se správnost fungování produktu.
- Případné chyby se uvedou do logu, kde se čeká na jejich opravu.

### Nasazení
- Proces uvádění hotového softwarového produktu do provozu v reálném prostředí

### Údržba
- V rámci údržby tým opravuje chyby, řeší problémy zákazníků a spravuje změny softwaru. Kromě toho tým monitoruje celkový výkon systému, bezpečnost a uživatelskou zkušenost, aby identifikoval nové způsoby, jak zlepšit stávající software.

# Waterfall
- Jedná se o základní model, první co vznikl v rámci vývoje software.
- Po dokončení jedné fáze, hned přechází dále.
- Je třeba důkladně pracovat na prvních fázích, aby nedošlo ke zmatku potom.

## Výhody
+ Jednoduchý model
+ Vhodný pro malé projekty

## Nevýhody
- Není flexibilní
- Nevhodný pro velké projekty
- Není cesty zpět na předchozí fázi
- Těžko se odhadují náklady a časová náročnost projektu

# Spirální model
- Proces vývoje, který kombinuje designový a prototypový přístup tak, aby postupoval v kombinování výhod od shora dolů (prototypování) a zdola nahoru (designování).
- Základní čtyři kvadranty modelu (iterace = jedno projití spirálou): 
  - Analýza
  - Vyhodnocení 
  - Vývoj 
  - Plánování

## Výhody
+ Flexibilita: Umí se přizpůsobit měnícím se požadavkům během vývoje.
+ Iterativnost: Opakované iterace umožňují postupné zlepšování a zdokonalování produktu.
+ Zahrnutí zákazníka: Průběžné prezentace a zpětná vazba od zákazníka jsou integrované do procesu.
+ Postupné zvyšování složitosti: Umožňuje postupné zvyšování složitosti produktu s každou iterací.
+ Včasná detekce chyb: Díky průběžnému testování mohou být chyby detekovány a opraveny dříve v procesu vývoje.

## Nevýhody
- Náklady: Implementace spirálového modelu může být nákladnější v porovnání s jednoduššími modely vývoje.
- Časová náročnost: Kvůli opakovaným iteracím a důrazu na analýzu a plánování může trvat déle než jiné modely dostat produkt na trh.
- Nemusí být vhodný pro malé projekty: Pro menší a méně komplexní projekty může být spiralový model příliš robustní a zdánlivě překomplikovaný.
- Nepředvídatelnost: Z důvodu neustálých změn a iterací může být obtížné předvídat časové a finanční nároky projektu

# Agilní přístup
- Agilní vývoj probíhá v krátkých cyklech, nazývaných iterace, které obvykle trvají několik týdnů.
- Každá iterace produkuje funkční část produktu, která může být okamžitě nasazena.
- Týmy pracují společně a pravidelně komunikují s klientem nebo uživateli, aby lépe porozuměli jejich potřebám a získali zpětnou vazbu.
- Agilní vývoj se snaží dodávat funkční části produktu od začátku vývoje, což umožňuje rychlou zpětnou vazbu od zákazníka.

## Výhody
- Rychlé dodání
- Průběžná zpětná vazba
- Flexibilita
- Efektivní spolupráce

## Nevýhody
- Složité vést dokumentaci
- Potřeba úzké spolupráce se zákazníkem
- Náročné plánování

## Scrum
- agilní, iterativní metodika vývoje

### Role
- Product Owner
  - Hlavní role Product Ownera je komunikace se zákazníkem. 
  - Je zodpovědný za obchodní stránku projektu. 
  - Do samotného vývoje však nezasahuje.
  - Ohlašuje uvedení nových verzí zákazníkovi, dohaduje priority, časový plán a financování.
- Scrum Master
  - Scrum Master je lídr týmu.
  - Dohlíží na dodržování dohodnutých procesů a je odpovědný za plynulé dodání produktových cílů.
  - Organizuje denní schůzky (tzv. denní scrum), kde se vyjadřuje k vývoji.
  - Jeho prioritou je též odstranění veškerých překážek, které týmu braní v dodání softwaru.
- Scrum Team Member
  - člen vývojářského týmu.

### Eventy
- Sprint Planning Meeting - plánování rozvržení práce pro Sprint na základě požadavků zákazníka (tzv. User Stories).
- Sprint - Iterace, která obvykle trvá dva až čtyři týdny. Začíná okamžitě po závěrech předchozího Sprintu.
- Daily Scrum (stand-up) - každodenní 15 minutové meetingy, konají se ve stejný čas, na stejném místě.
- Sprint Review - Scrum Team prezentuje zákazníkovi výsledný software, zákazník se k verzi vyjádří a pokud nebude spokojený, začíná nový Sprint.
- Sprint Retrospective - cílem je zjistit, jak je možné vývoj zefektivnit a zkvalitnit.

# Extrémní programování (XP)
- všechno je vedeno do extrémů
- odvážný přístup k vývoji, rychlost iterace (v řádu minut či hodin)
- párové programování (dva nebo více vývojářů u jednoho počítače)
- použijeme pokud nestíháme dokončit zakázku
- intenzivní testování
- není zaměřen na management

# Prototypovací model
- Prototypování je realizace projektu pomocí vytváření prototypů aplikací = neúplných verzí směřujících ke konečnému výsledku.
- Používá se za široce známou metodu (strojírenství, výroba, …)
- Obvykle je smyslem prototypování simulovat určitou část hotového produktu (může dojít i k tomu, že se prototyp bude výrazně lišit od celku)
- Účel: umožnit budoucím uživatelům SW hodnotit návrh designu a funkcí pomocí skutečného použití, nejen interpretace a komentování popisu produktu.

## Obecné fáze prototypování
1. Identifikace základních požadavků
2. Vývoj prvotního prototypu
3. Revize, zhodnocení, zpětná vazba
4. Pozměnění a vylepšení prototypu
5. Kroky 3 a 4 se opakují podle potřeby několikrát.

## Druhy prototypů
- horizontální prototyp: 
  - První návrh UI
  - Slouží k náhledu na celý system nebo subsystém 
  - Hlavním účelem je demonstrace komunikace s uživatelem spíše než funkčnost
- vertikální prototyp:
  - úplnější propracování jednoho podsystému nebo funkce produktu
  - je vhodné pro získání lepších požadavků na danou funkci: zjemnění návrhu databáze, informace o objemu dat a výkonnostních potřebách
  - zjednodušení složitých požadavků

## Typy prototypování
- **zahazovací prototypování (rapidní prototypování)** 
   - Vytvoření modelu, co nebude součásti projektu.
  - Model bude zahozen a využit k reprezentaci požadované funkce zákazníkovi.
  - Následně se využije jako návrh k ostré verzi.
  - Model slouží jako východisko pro zpětnou vazbu od zákazníka.
  - Na základě sebraných poznatků tvoří se finální verze.

- **evoluční prototypování**
  - Vyvinutý model je potom použít jako jádro
  - Zákazník dostane verzi a může se k tomu vyjádřit
  - Postupně jsou provedeny nové úpravy a features
  - In podstatě nejde o “finální” produkt, vždy se najde nějaká chyba, která je pak vyřešená, nebo nový požadavek

- **inkrementální prototypování**
    - produkt se skládá z dílčích prototypů, které na závěr slučujeme na výsledné řešení.

- **extrémní prototypování**
  - dělí se na 3 fáze, každá vychází z té předchozí
  - zaměřuje se především na Web development
  - První fáze je statický prototyp
  - Druhá fáze je kódování funkčního
  - Třetí fáze je implementace funkcí
  - V podstatě nejde o “finální” produkt, vždy se najde nějaká chyba, která je pak vyřešená, nebo nový požadavek

# RUP (Rational Unified Process)
- Iterativní a inkrementální, tradiční a striktní přístup.
- Vhodná pro velké projekty pro firmy s větším počtem zaměstnanců (korporáty, banky).
- Striktně sestaví požadavky a po konci iteraci jsou definované nové požadavky.
- Obsahuje tyto 4 fáze: 
  - Zahájení - sjednocení potřeby celého projektu, jeho proveditelnost a vhodnost. Nápad, struktura projektu je definována.
  - Rozpracování - analýza požadavků, tvorba podrobných specifikací, návrh architektury, vytvoření plánu projektu.
  - Konstrukce - implementace, testování, integrace, vytvoření dokumentace.
  - Předání - nasazení, údržba, podpora, vytvoření dokumentace.

- Po dokončení iterace začne se další až nebude zákazník spokojen.

## Popis činnosti
- **Business modelování** - popsat strukturu a dynamiku podniku či organizace. (kdo co dělá)
- **Požadavky** - stanovení, dokumentace požadavků od zákazníka
- **Analýza a design** - návrh software, UML diagramy, návrh databáze
- **Implementace** - samotná tvorba zdrojového kódu / databáze
- **Testování** - testování softwaru
- **Nasazení** - nasazení hotového softwaru

## Výhody
* Iterativní, snadné odhalení chyb
* Důkladné vypracování dokumentace, UML
* Snazší správa změn

## Nevýhody
- Nevhodný pro malé projekty
- Nákladný na impolementaci

# Zdroje a Zajímavé Odkazy
Seznam použitých zdrojů a případně odkazy na další zajímavé informace k tématu


