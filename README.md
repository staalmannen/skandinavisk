# skandinavisk

Kompletterande språkresurser och tekniska integrationer för [Nordum](https://nordum.org/), ett gemensamt skandinaviskt skriftspråk.

## Syfte

Skandinavisk är ett tekniskt kompletteringsprojekt med Nordum som uppströms språklig referens. Vi vill göra Nordum användbart i fler program, operativsystem och digitala arbetsflöden genom att utveckla och underhålla språkresurser och integrationer som saknas eller behöver kompletteras.

Projektet har därmed inte längre som huvudmål att utveckla en konkurrerande skandinavisk språkstandard. Nordums specifikation, ordlista och språkliga arbete är utgångspunkten för våra resurser.

## Prioriteringar

1. **Stavningskontroll:** Hunspell-ordlista och affixregler, med tester för ordformer och böjningar.
2. **Synkronisering:** reproducerbar hämtning och versionslåsning av relevanta Nordum-data.
3. **Programintegrationer:** språkstöd för kontorsprogram, texteditorer och andra verktyg.
4. **Systemresurser:** locale-data, språkidentifiering och relaterade operativsystemresurser där det är relevant.
5. **Språkteknologi:** korpusar, testmaterial och andra maskinläsbara resurser.

Översättningsfiler är en del av uppdraget, men projektets omfattning är bredare: även ordlistor, böjningsregler, tester och integrationsmetadata behövs.

## Förhållandet till Nordum

- Nordum är uppströms källa för språkets norm, grammatik och grundläggande ordförråd.
- Skandinavisk återanvänder Nordums arbete i stället för att duplicera det.
- Vi dokumenterar källor, versioner och licenser för allt återanvänt material.
- Tekniska anpassningar ska hållas åtskilda från språkliga förändringar.
- Förslag som påverkar själva språket ska motiveras, dokumenteras och när det är lämpligt föras vidare till Nordum.
- Skandinavisk är ett självständigt kompletteringsprojekt; detta dokument förutsätter inte att Nordum formellt har godkänt eller antagit någon sådan relation.

Se [projektets relation till Nordum](planering/forhallande-till-nordum.md) för arbetsprinciper och [den tekniska färdplanen](planering/teknisk-fardplan.md) för planerade leveranser.

## Projektstruktur

- [hunspell/](hunspell/README.md) – stavningskontroll och ordlistor.
- [forskning/](forskning/) – undersökningar och jämförande underlag.
- Övriga tekniska kataloger skapas när det finns konkret innehåll att lägga där.

## Arbetssätt

- Följ Nordums aktuella specifikation och versionshantera importerade data.
- Gör byggen och tester reproducerbara.
- Håll källmaterial, genererade filer och lokala anpassningar åtskilda.
- Redovisa licens och attribution för varje extern datakälla.
- Markera tydligt vad som är implementerat, experimentellt respektive planerat.

## Status

Projektet befinner sig i en omställning från ett självständigt språkstandardiseringsinitiativ till ett tekniskt kompletteringsprojekt kring Nordum. Första konkreta mål är att utreda och ta fram Hunspell-stöd.
