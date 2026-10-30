# Övning: Receptsajten

Under kursens fyra första veckor bygger du **en egen liten receptsajt**. Du utgår från
receptsidan med pannkakor från test- och kartläggningen. Efter de första veckorna blir den till en större sajt som är tillgänglig, responsiv och byggd med CSS som någon annan kan läsa och arbeta vidare på.

Det här är **ingen inlämningsuppgift**. Den kommer efteråt och bygger på samma kunskaper. Här
övar du på det vi går igenom under veckorna.

## Varför de här veckorna?

Allt du lär dig här kommer du att ha nytta av i varje framtida projekt, oavsett vilket ramverk du landar i:

- **Tillgänglighet från början.** En sajt är inte klar förrän alla kan använda den, med
  tangentbord, skärmläsare eller förstorad text. Det är mycket lättare att bygga in det från
  början än att laga det i efterhand, och semantisk HTML gör det mesta av jobbet.
- **Vanliga mönster.** Meny, kort i en grid, en stor bild med rubrik, ett formulär: samma byggstenar
  finns på nästan varje sajt. Kan du bygga dem väl och förstår varför de är uppbyggda som de är,
  kan du bygga det mesta.
- **Kod som håller.** Koden ska gå att läsa, ändra och bygga vidare på, av dig om ett halvår eller
  av en kollega i morgon. Tokens, tydlig namngivning och flexibel layout i stället för fasta mått
  gör att en ändring på ett ställe inte förstör tre andra.
- **Medvetna val som du kan förklara.** Det finns oftast flera sätt att lösa samma sak, till
  exempel flex eller grid, `rem` eller `px`, en klass eller en selector. Det viktiga är att du
  väljer medvetet och kan säga varför. Det är det fredagarnas kodsnack övar.

## Veckoplan

Undervisningen följer den här planen, och kolumnen "Sajten efter veckan" är **det minsta alla ska
ha gjort** till veckans fredag. Kodsnacket utgår från det, så alla behöver ha det med sig. Om du
hinner mer får du gärna gå vidare till nästa vecka, gå tillbaka och förbättra det du redan gjort
eller ta dig an något under [Extra](#extra).

| Vecka | Fokus                              | Sajten efter veckan                                                                                                                                                                                                                                  | Till kodsnacket (fredag)                                                       |
| ----- | ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| 1     | Semantik och tillgänglighet        | Pannkakssidan har samma innehåll som förut men semantisk HTML: bilder med genomtänkta alt-texter och bildtexter där de behövs, fakta i `dl`, ingredienser som en lista med checkboxar och steg i `ol`. Den klarar WAVE, tangentbord och skärmläsare. | Visa sidan i WAVE och berätta vad du ändrade och varför.                       |
| 2     | Designsystem och ren CSS           | Sidan har en egen stil med en reset, tokens och typsnitt. Ingredienser du bockar av stryks över med `:has()`, och hover- och fokuslägen är tydliga.                                                                                                  | Granska varandras CSS och formulera gemensamma principer för "ren CSS".        |
| 3     | Box model, flex och grid           | Sidan har blivit en sajt, med meny, en startsida med bild, kategorier och kort, och två kolumner på receptsidan.                                                                                                                                     | Visa var du använt flex och grid, och hur layouten beter sig på olika skärmar. |
| 4     | Responsivt, formulär, färg och Git | Sajten är komplett: sidan Dela recept är på plats, alla sidor fungerar från 300 till 1920px, färgsystemet är klart och koden ligger på GitHub.                                                                                                       | Förklara en annan deltagares kod, med fokus på formuläret.                     |

Veckans mål och material finns i planeringen och visar mer i detalj vad du kan ta med i varje
steg.

## Ramar

- Använd bara HTML och CSS, alltså inga bibliotek, ramverk eller JavaScript.
- Om du lånar en reset, ett utility eller liknande ska du skriva källan i en kommentar.
- Lägg upp koden i ett publikt repo på din GitHub senast torsdag vid dagens slut i vecka 4. Då
  hinner de andra i gruppen läsa din kod innan kodsnacket på fredagen.
- Var beredd på att förklara din kod. Om du tar hjälp av andra eller av AI måste du förstå vad
  koden gör och ha kunskapen för att reproducera den självständigt.

---

## Slutmålet: så här ser sajten ut när den är klar

```
Receptsajten
├── Startsida     bild med rubrik, kategorier och receptkort som länkar vidare
├── Receptsida    pannkakor: fakta, ingredienser att bocka av och steg
└── Dela recept   ett formulär där besökaren skickar in ett eget recept

Finns på alla sidor: samma meny, samma footer och samma designsystem
```

Skisserna nedan är **förslag** för stor skärm. De visar innehåll och struktur, inte exakt utseende. Välj
själv färger, typsnitt och detaljer, och byt gärna ut delar mot något som övar samma sak.

> **Så läser du skisserna**
>
> - `_text_` är en länk
> - `[text]` är en knapp eller en länk som ser ut som en knapp
> - `(text)` är en tagg
> - `[____]` är ett fält i ett formulär
> - `( )` är en radioknapp
>
> Text utan tecken runt är vanlig text.

### Startsidan

Bara pannkakssidan behöver finnas på riktigt. Låt alla receptkort länka till den, och använd
`href="#"` för länkar till sidor som inte finns, t.ex. kategorierna och Om sajten.

```
┌──────────────────────────────────────────────┐
│ LOGO      _Recept_ _Om sajten_ [Dela recept] │
├──────────────────────────────────────────────┤
│ ┌──────────────────────────────────────────┐ │
│ │ ░░░░░░░░░░░░░░ bild ░░░░░░░░░░░░░░░░░░░░ │ │
│ │   Rubrik och intro ovanpå bilden         │ │
│ └──────────────────────────────────────────┘ │
│ (Frukost) (Middag) (Efterrätt) (Fika)        │
│ ┌────────────┐ ┌────────────┐ ┌────────────┐ │
│ │    bild    │ │    bild    │ │    bild    │ │
│ │_Pannkakor_ │ │_Receptnamn_│ │_Receptnamn_│ │
│ │ 30 min     │ │ 45 min     │ │ 15 min     │ │
│ └────────────┘ └────────────┘ └────────────┘ │
├──────────────────────────────────────────────┤
│ LOGO                      _Om sajten_        │
│ Enkla vardagsrecept som                      │
│ alla kan laga.            Fler recept        │
│                           _Frukost_          │
│                           _Middag_           │
│                           _Efterrätt_        │
│                           _Fika_             │
│ Bilder från picsum.photos · © 2026 Ditt namn │
└──────────────────────────────────────────────┘
```

### Receptsidan

Receptsidan är den du redan har gjort. **Behåll innehållet, men gör om layouten enligt skissen.**
Det enda nya innehållet är fakta om receptet. Tid och svårighetsgrad hittar du på själv.

```
┌──────────────────────────────────────────────┐
│ meny                                         │
├──────────────────────────────────────────────┤
│ ┌──────────────────┐  Enkelt recept på       │
│ │   stor bild på   │  pannkakor (h1)         │
│ │    pannkakor     │  Gör traditionella      │
│ │                  │  tunna pannkakor ...    │
│ │                  │  ┌──────┬──────┬──────┐ │
│ │                  │  │4 port│30 min│ Lätt │ │
│ └──────────────────┘  └──────┴──────┴──────┘ │
│ Ingredienser          Så här gör du          │
│ För 4 portioner       1. Blanda mjöl och     │
│ ☑ 2 1/2 dl vetemjöl      salt i en bunke.    │
│ ☑ 1/2 tsk salt        2. Vispa i hälften     │
│ ☐ 6 dl mjölk             av mjölken ...      │
│ ☐ 3 ägg               3. ...                 │
│ ☐ ...                 6. Servera med sylt,   │
│                          bär eller frukt.    │
│ Serveringsförslag                            │
│ ┌───────────────────┐ ┌───────────────────┐  │
│ │        bild       │ │        bild       │  │
│ ├───────────────────┤ ├───────────────────┤  │
│ │ Med sylt & grädde │ │ Med apelsin       │  │
│ └───────────────────┘ └───────────────────┘  │
├──────────────────────────────────────────────┤
│ footer                                       │
└──────────────────────────────────────────────┘
```

### Dela recept

Formuläret har en kolumn på alla skärmar, så skissen gäller både desktop och mobil. `*` betyder
att fältet är obligatoriskt, och sista fältet visar hur ett ogiltigt fält ser ut när man har
lämnat det (`:user-invalid`).

```
┌──────────────────────────────────────────────┐
│ meny                                         │
├──────────────────────────────────────────────┤
│ Dela ditt recept (h1)                        │
│ Kort intro till formuläret                   │
│                                              │
│ ┌ Om receptet ─────────────────────────────┐ │
│ │ Receptets namn *                         │ │
│ │ [______________________________________] │ │
│ │ Kategori                                 │ │
│ │ [Välj kategori                        ▼] │ │
│ │ Tid i minuter        Antal portioner     │ │
│ │ [_______]            [_______]           │ │
│ └──────────────────────────────────────────┘ │
│ ┌ Svårighetsgrad ──────────────────────────┐ │
│ │ ( ) Lätt    ( ) Medel    ( ) Svår        │ │
│ └──────────────────────────────────────────┘ │
│ ┌ Receptet ────────────────────────────────┐ │
│ │ Ingredienser *                           │ │
│ │ [______________________________________] │ │
│ │ [______________________________________] │ │
│ │ Gör så här *                             │ │
│ │ [______________________________________] │ │
│ │ [______________________________________] │ │
│ └──────────────────────────────────────────┘ │
│ ┌ Om dig ──────────────────────────────────┐ │
│ │ Ditt namn                                │ │
│ │ [______________________________________] │ │
│ │ E-post *                                 │ │
│ │ [anna@_________________________________] │ │
│ │ ✗ Ange en giltig e-postadress            │ │
│ └──────────────────────────────────────────┘ │
│                                              │
│ [Skicka recept]                              │
├──────────────────────────────────────────────┤
│ footer                                       │
└──────────────────────────────────────────────┘
```

> **Formuläret behöver inte fungera på riktigt.** Det ska inte skicka eller spara något
> någonstans, för det kräver en server, och det ingår inte i övningen. Det som räknas är HTML:en,
> tillgängligheten, valideringen i webbläsaren och stylingen. När alla fält är giltiga och du
> trycker på knappen laddas sidan om och fälten töms. Det är väntat och inget fel.

## Det här ska sajten visa att du kan

Använd listan som checklista. Det är de här målen sajten ska uppfylla när de fyra veckorna är
slut. [Veckoplanen](#veckoplan) visar vad som ska vara klart till varje fredag.

**Struktur och tillgänglighet**

- Semantisk HTML: landmarks (`header`, `nav`, `main`, `footer`), `section` och `article` där det
  passar, en `h1` per sida och rubriker i logisk ordning. Receptdetaljer använder passande element
  (t.ex. lista med kryssrutor för ingredienser, `ol` för steg, `dl` för fakta).
- Bilder har genomtänkta alt-texter (`alt=""` för dekorativa). `figure` och `figcaption` används
  där en synlig bildtext tillför värde (t.ex. på serveringsförslagen).
- Menyn visar vilken sida du är på med `aria-current="page"`. Om footern har en egen `nav` har den
  en särskiljande `aria-label`.
- Sajten går att använda med bara tangentbordet, fungerar med en skärmläsare och ger inga fel i
  WAVE.

**CSS som håller**

- Sajten har en CSS reset, och källan står i en kommentar.
- Färger, typsnitt och avstånd ligger i variabler (tokens), och det finns inga hårdkodade färger.
- Du har en genomtänkt enhetsstrategi (`rem`, `px`), och sidan klarar 200 % textstorlek utan att
  innehåll klipps.
- Tydliga selectors och klassnamn utan `!important`, t.ex. `li:has(:checked)` som stryker över
  ingredienser du har bockat av.
- Tydliga `:hover`- och `:focus-visible`-lägen för interaktiva element.

**Layout**

- Box-modellen används medvetet (`box-sizing: border-box`) med god förståelse för när du ska använda `padding` respektive `margin`. Använd gärna logical properties (t.ex. `padding-inline` och `margin-block`).
- Medvetna val mellan Flexbox och Grid: använd Flexbox när innehållets storlek och naturliga flöde ska styra (t.ex. meny, kategorier eller inuti korten) och Grid när behållaren ska sätta upp en tydlig struktur med kolumner och spår (t.ex. receptkorten eller receptsidans sektioner). Du ska kunna motivera dina val.
- På startsidan ligger rubriken ovanpå bilden i hero-sektionen. Testa i första hand att lösa överlappningen med grid (genom att låta bild och text dela samma cell), men blir det för krångligt kan du använda `position: absolute`.
- Koden har inga onödiga wrapper-`div`:ar och inga låsande fasta höjder.

**Responsivitet och färg**

- Sajten bygger på flytande design snarare än brytpunkter och ser bra ut från ca 300px till ca 1920px:
  - Menyn och kategorierna bryts naturligt med `flex-wrap` (ingen hamburgermeny behövs).
  - Receptkorten byter antal kolumner flytande med `repeat(auto-fit, minmax(...))`, helt utan media queries.
  - Typografi och avstånd skalar flytande med `clamp()`, `min()` och `max()` i stället för fasta hopp vid brytpunkter.
  - Du får använda media queries om det behövs, men undvik dem när du kan och sträva efter mer dynamiska lösningar i första hand.
- Färgerna är satta med ett modernt färgsystem (t.ex. `oklch()` eller `hsl()`) och har god kontrast (WCAG AA), även för texten ovanpå bilden.

**Formulär**

- Varje fält har en kopplad `label`, och fält som hör ihop är grupperade med `fieldset` och `legend`.
- Fälten har rätt `type`, `required` där det behövs, samt tydlig visuell feedback för giltiga och
  ogiltiga fält (`:user-valid` / `:user-invalid`).

## Extra

<details>
<summary><strong>För dig som vill ha mer utmaning (klicka för att fälla ut)</strong></summary>

Här är några idéer och tips att arbeta vidare med:

- en skip link högst upp på sidan
- fler riktiga receptsidor (bra om du vill nöta in kunskap eller repetera för dig själv)
- kategorier som filtrerar korten med bara CSS (`radio` och `:has()`)
- textfält i formuläret som växer automatiskt med innehållet (`field-sizing: content`)
- en meny som följer med när man scrollar (`position: sticky`). Se till att den inte döljer det
  som har fokus när man tabbar, t.ex. med `scroll-padding-top`.
- en diskret `transition` på hover och focus-visible
- mörkt läge med `light-dark()`
- ett utvalt recept, t.ex. "Veckans recept", som tar mer plats i griden. Styla det utifrån
  innehållet med `:has()` eller ett data-attribut, i stället för med en extra klass.
- receptkort som anpassar sig efter sin egen bredd i stället för skärmens, med container queries
  ([MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Containment/Container_queries),
  [Kevin Powell](https://www.youtube.com/watch?v=2rlWBZ17Wes))
- en sidlayout med namngivna grid-linjer i stället för wrapper-klasser, där delar kan gå utanför
  textbredden eller kant i kant
  ([Kevin Powell](https://www.youtube.com/watch?v=c13gpBrnGEw),
  [färdig kod](https://codepen.io/kevinpowell/pen/ExrZrrw))
- en sajt som är lättare att hitta i sökmotorer, med `<title>`, `<meta name="description">` och
  strukturerad data för receptet
  ([Googles SEO-startguide](https://developers.google.com/search/docs/fundamentals/seo-starter-guide),
  [Recipe i JSON-LD](https://developers.google.com/search/docs/appearance/structured-data/recipe))

</details>

## Övriga resurser

- Bilder kan du hämta från [picsum.photos](https://picsum.photos/) eller ta egna.
- Länkar som inte har någon sida ännu ska ändå vara semantiska, använd `href="#"`.
