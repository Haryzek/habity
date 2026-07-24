# Habity — návod pro uživatele

Osobní tracker návyků, úkolů a pohybu. Běží v prohlížeči, **všechna data jsou
jen ve tvém zařízení** (localStorage prohlížeče). Nikam se neposílají, není účet,
není přihlášení. Zároveň: **když smažeš data prohlížeče, je to pryč** — proto
občas exportuj zálohu (viz konec).

Tip: v mobilním prohlížeči dej „Přidat na plochu" — chová se pak jako appka.

---

## Jak se v tom pohybuješ

**Dole je 6 tlačítek = 6 sekcí:** Litánie · Progress · Tasks · Habits · Free · Move.

**Švihnutím prstem doleva/doprava** přepínáš uvnitř sekce mezi dvěma rovinami:
- **Check** — dnešek, tady se odškrtává,
- **Přehled** — historie jako mřížka čtverečků.

Kde jsi, poznáš podle dvou teček nahoře (dají se i naklikat). Habits a Free
otevírají rovnou Přehled, ostatní Check. Move a Litánie mají jen jednu plochu.

**Kulaté „+" vpravo dole** přidá položku do právě otevřené sekce.
**Ozubené kolečko ⚙ nahoře** = záloha, import a mazání historie.

---

## Sekce

### Tasks — úkoly s termínem
Hlavní obrazovka appky. Shora **WiP náhled** (nedatované úkoly, co tě čekají),
pod ním **kalendář** po dnech (Dnes, Zítra, …).

U každého úkolu v kalendáři jsou čtyři akce:
- **✓** splněno — přiletí 🍹 a den dostane zelený čtvereček,
- **→** posun na zítřek, **»** na příští týden — bez trestu, nic se nezaznamená,
- **✕** nesplněno — dobrovolné přiznání, den dostane červený čtvereček.

**Klik na název úkolu** = editace. Tam nastavíš prioritu (1–10), termín
(Dnes / Zítra / datum), **opakování** (denně až ročně) a **backlog** (kýbl, do
kterého úkol patří). Když nedáš žádný termín, úkol spadne do backlogu a čeká.

**Opakující se úkoly:** po odškrtnutí se samy naplánují znovu. Buď klouzavě od
dne splnění (necháš „bouncer" prázdný), nebo v pevném rytmu podle zadaného dne
(např. blog vždy ve středu, záloha na daň vždy 15. 6.).

Backlogy přepínáš rozbalovací lištou nahoře („Wip"). „Wip" = rozdělané, „Done" =
archiv splněných, „Future" = někdy potom. Vlastní si přidáš tlačítkem
„+ nový backlog"; přejmenovat/smazat jde tužtičkou a ✕ přímo ve výběru.

**Červené čtverečky** vznikají jen dvěma způsoby: buď dáš ✕, nebo necháš
neopakující se úkol propadnout přes půlnoc. Odsouvání ani opakující se úkoly
červenou nikdy nedělají. Přehled je tak upřímný přesně tak, jak upřímný jsi ty.

**Přehled** (švihni doleva) ukazuje po dnech nebo po měsících, kolik toho bylo
zeleného a kolik červeného.

### Habits — návyky
Check rovina = dnešní odškrtávání. Přehled = mřížka 30 dnů zpátky pro každý
návyk; **klikáním přímo do čtverečků** zapisuješ i zpětně. Klik na název bloku
otevře editaci návyku, klik na čísla vpravo celkovou historii od začátku.

### Free — volnočasové návyky
To samé jako Habits, navíc **backlogy** (rozbalovátko nahoře třídí seznam),
**vyhledávání** a **filtry podle štítků**. Přehled agreguje všechno napříč
backlogy.

### Progress — projekty s kroky
Pro věci, co mají víc kroků (např. „Stěhování bytu"). Projekt = placka,
rozklikneš ji a odškrtáváš kroky. Každý krok má **N** (náročnost) a **P**
(prioritu) — náročnost určuje, jak velký kus proužku postupu krok ukrojí,
priorita jen pořadí ve výpisu. Šedé **+** na placce rovnou přidá další krok.
Když je projekt na 100 %, objeví se u něj 🍹.

Bonus: v editaci úkolu v Tasks můžeš přes „→ projekt…" úkol překlopit rovnou
jako krok nějakého projektu.

### Move — pohyb z Garminu
Každý den = jedno kolečko, řádek = týden (pondělí vlevo, nejnovější nahoře).
- **velikost kolečka** = spálené kalorie,
- **číslo uvnitř** = minuty pohybu,
- **zelená levá půlka prstence** = vzdálenost,
- **červená pravá půlka** = tep.

Prázdný den = jen tečka. Data se plní automaticky ze zaznamenaných aktivit
(tohle je napojené na Bobův Garmin — u tebe se sekce naplní, jen když si stejnou
pipeline postavíš). **Klik na kolečko** otevře ruční zadání čtyř čísel — takhle
zadaný den se zamkne (kalorie kurzívou) a automatika ho už nepřepíše.

### Litánie — podpůrné věty
Knihovna vlastních vět, přerámování a manter s tagy, prioritou 1–5, hvězdičkou
pro oblíbené a očičkem 👁 na označení „už jsem to prošel". Filtruješ chipy,
fulltextem a sliderem priority. Mazání není doopravdy mazání — věta se jen
schová a jde vrátit („Vrátit" v liště, která na pár vteřin vyskočí).

Obsah je čistě soukromý a nikde se nestahuje — sekce je prázdná, dokud si do ní
nenaimportuješ vlastní data.

---

## Zálohování (čti to)

⚙ → **Exportovat zálohu** stáhne `habity-zaloha.json` s úplně vším. Importem ho
kdykoli naleješ zpátky přes **Načíst zálohu ze souboru**. Dělej to pravidelně a soubor si někam odlož (Dropbox,
disk) — jiná kopie tvých dat neexistuje.

⚙ → **Vymazat historii úkolů** smaže jen čtverečky v Přehledu, ne samotné úkoly.
