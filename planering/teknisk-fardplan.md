# Teknisk färdplan

**Status:** prioriteringsförslag för Skandinavisk som tekniskt kompletteringsprojekt kring Nordum.

## Målbild

Bygga återanvändbara språkresurser och integrationer som gör Nordum tillgängligt i program och system där stödet saknas eller behöver förbättras. Arbetet ska i första hand utgå från Nordums publicerade data och specifikation.

## Etapp 1 – Hunspell

Första prioritet är en fungerande stavningskontroll för Nordum.

Arbetsmoment:
1. undersök Nordums ordlista, specifikation och eventuella API:er eller exportformat,
2. identifiera hur böjningar och ordklasser representeras,
3. inventera de svenska och danska Hunspell-källor som redan finns i repositoryt och kontrollera deras licenser,
4. definiera en reproducerbar pipeline från upstream-data till Hunspell,
5. skapa en första ordlista och affixfil,
6. bygg tester för accepterade ord, böjningar och vanliga felstavningar,
7. dokumentera begränsningar och kompatibilitet.

**Leverans:** ett testat och versionsmärkt Hunspell-paket som tydligt anger vilken Nordum-version det bygger på.

## Etapp 2 – robust upstream-flöde

- versionslås källmaterial till release eller commit,
- automatisera hämtning och konvertering där det är möjligt,
- separera upstream-data från lokala korrigeringar och genererade filer,
- skapa kontroller som upptäcker ändringar i källformat eller orddata,
- dokumentera licens och proveniens.

## Etapp 3 – fler integrationer

Välj nästa integration utifrån efterfrågan och underhållbarhet. Möjliga områden:

- LibreOffice och andra kontorsprogram,
- texteditorer och utvecklingsmiljöer,
- locale-data och språkidentifiering,
- översättnings- och lokaliseringsfiler,
- andra stavnings- och grammatikkontrollsystem.

## Etapp 4 – språkteknologiska resurser

När grunddata och byggflöden är stabila kan vi undersöka:
- testkorpusar och regressionsmaterial,
- frekvenslistor och terminologiresurser,
- tokenizer- och språkidentifieringsstöd,
- andra maskinläsbara resurser för NLP och AI.

## Prioriteringskriterier

Nya uppgifter bör bedömas efter:
- om behovet inte redan täcks av Nordum,
- hur många program och användare som kan dra nytta av resultatet,
- om upstream-data och licenser medger återanvändning,
- hur reproducerbar och testbar lösningen blir,
- långsiktig underhållskostnad.

## Vad som inte längre är huvuduppdrag

Att utveckla en egen konkurrerande stavningsstandard, grammatik eller kärnordlista är inte längre Skandinavisk-projektets mål. Språkliga förbättringsförslag kan dokumenteras och föras vidare till Nordum, men tekniskt integrationsarbete är vår huvudsakliga leverans.
