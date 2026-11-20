# Förhållandet till Nordum

**Status:** arbetsprincip för Skandinavisk. Dokumentet beskriver vår avsedda arbetsmodell och innebär inte att Nordum formellt har godkänt eller antagit en dotterprojektrelation.

## Rollfördelning

Nordum är det uppströms projektet för det gemensamma skandinaviska skriftspråket. Nordums specifikation, grammatik, ordlista och språkliga beslut är utgångspunkten för Skandinavisk.

Skandinavisk är ett kompletterande tekniskt projekt. Vårt uppdrag är att utveckla och underhålla språkresurser, format och integrationer som gör Nordum användbart i fler program och tekniska miljöer.

Relationen kan beskrivas som ett dotterprojekt eller ett downstream-projekt i teknisk mening: vi bygger vidare på Nordums arbete, men är fortsatt ett självständigt repository och en självständig arbetsyta.

## Vad vi återanvänder

I första hand återanvänder vi, med respekt för respektive licens och villkor:

- Nordums språk- och stavningsspecifikation,
- Nordums ordlista och terminologiska data,
- dokumenterade böjnings- och grammatikregler,
- befintliga maskinläsbara data och exportformat,
- relevanta tester och verktyg som Nordum publicerar.

Vi ska föredra att hämta eller generera från en tydligt versionslåst upstream-källa framför att manuellt kopiera och underhålla dubbla datamängder.

## Tekniska anpassningar och språkliga avvikelser

Vi skiljer mellan tre slags förändringar:

1. **Direkt återanvändning:** Nordums former och regler återges oförändrade.
2. **Teknisk anpassning:** data omformas för ett visst format eller program utan att språkets norm ändras. Exempel kan vara Hunspell-format, locale-metadata eller begränsningar i ett översättningsformat.
3. **Språklig avvikelse eller ändringsförslag:** en lokal resurs använder en annan stavning, böjning eller ordform än Nordum.

Tekniska anpassningar ska hållas i integrationslagret när det är möjligt. Språkliga avvikelser ska inte smygas in som om de vore Nordums officiella former.

Varje föreslagen språklig avvikelse ska dokumentera:
- Nordums aktuella form och källa,
- den föreslagna alternativa formen,
- konkreta exempel,
- motiv och förväntad nytta,
- konsekvenser för begriplighet och kompatibilitet,
- om förslaget har framförts till Nordum och eventuell återkoppling.

När det är lämpligt ska förslag som påverkar själva språket föras vidare till Nordum. Skandinavisk kan behöva behålla en lokal anpassning för ett specifikt tekniskt ändamål, men den ska då märkas och versionshanteras som sådan.

## Licenser och proveniens

Publikt tillgängligt material är inte automatiskt fritt att kopiera. Innan vi återanvänder kod, ordlistor, texter eller andra data ska vi kontrollera licensen för just den resursen och följa krav på attribution, delning och kompatibilitet.

För varje importerad källa ska vi om möjligt registrera:
- projekt och exakt käll-URL,
- fil eller dataset,
- version, release eller commit,
- hämtningsdatum,
- licens och attribution,
- eventuella lokala ändringar.

Nordums webbplats och repository kan ha olika licensvillkor för olika material. Licens ska därför kontrolleras på resursnivå.

## Kommunikation

Vi bör vara öppna med att Skandinavisk bygger på Nordums arbete. Vi ska inte ge intryck av att vara officiellt sanktionerade av Nordum utan uttryckligt besked. När vi upptäcker fel, luckor eller förbättringsmöjligheter bör vi rapportera dem konstruktivt upstream.

## Praktisk tumregel

Om ett problem kan lösas genom att förbättra importen, konverteringen, testningen eller integrationen ska vi göra det där. Om lösningen kräver att själva språket ändras ska vi först dokumentera avvikelsen och överväga att föreslå ändringen till Nordum.
