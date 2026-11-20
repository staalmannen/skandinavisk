# Projektets mål och grundprinciper

**Aktuell inriktning:** tekniskt kompletteringsprojekt kring Nordum.

## Övergripande mål

Skandinavisk ska utveckla, paketera och underhålla språkresurser och tekniska integrationer för Nordum. Målet är att göra språket tillgängligt i program, operativsystem och digitala arbetsflöden där Nordums egna verktyg eller resurser ännu inte täcker behovet.

Nordums publicerade specifikation, grammatik och ordförråd är vår uppströms språkliga referens. Skandinavisk ska i första hand återanvända och bygga vidare på detta arbete, inte utveckla en parallell språkstandard.

## Arbetsområden

- stavningskontroll, bland annat Hunspell,
- ordlistor, affixregler och böjningsdata,
- översättnings- och lokaliseringsfiler,
- integrationer för kontorsprogram och texteditorer,
- locale- och systemresurser,
- testkorpusar och kvalitetssäkring,
- andra maskinläsbara språkresurser som underlättar praktisk användning.

## Förhållandet till språknormen

Nordums aktuella norm är utgångspunkten. Vi ska dokumentera vilken version av specifikationen och vilka källor varje resurs bygger på.

Tekniska begränsningar kan ibland kräva anpassningar. Sådana ska i första hand lösas i integrationslagret och inte genom att ändra språkets stavning eller grammatik.

Om en språklig avvikelse verkar nödvändig ska den:
1. beskrivas tydligt och med konkreta exempel,
2. motiveras utifrån begriplighet, konsekvens eller tekniska behov,
3. hållas åtskild från Nordums officiella former,
4. om lämpligt framföras som ett förslag till Nordum.

En lokal anpassning blir inte automatiskt en ändring av Nordums norm.

## Kvalitetsprinciper

- **Spårbarhet:** varje importerad eller bearbetad resurs ska ha dokumenterad källa och version.
- **Licensmedvetenhet:** återanvändning ska följa respektive källas licens och krav på attribution.
- **Reproducerbarhet:** genererade resurser ska kunna byggas om från dokumenterade källor och skript.
- **Testbarhet:** ordlistor och regler ska ha automatiserade tester där det är möjligt.
- **Åtskillnad:** upstream-data, lokala anpassningar och genererade artefakter ska hållas isär.
- **Samarbete:** förbättringar som berör själva språket bör återkopplas till Nordum när det är lämpligt.

## Första prioritering

Första konkreta leveransen är att undersöka Nordums ordlista och böjningsmodell och jämföra dem med de Hunspell-resurser som redan finns i repositoryt. Resultatet ska ligga till grund för en testbar Hunspell-implementation.
