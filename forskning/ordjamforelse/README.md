# Jämförelse av de vanligaste orden i svenska, danska och norska

**Status:** forskningsplan och datakällor identifierade. Inga nya kognatprocent är ännu beräknade.

## Forskningsfråga

Hur stor del av det vanligaste ordförrådet i svenska, danska och norska är gemensamt eller historiskt besläktat – och hur stor del är dessutom likt till formen och betydelsen?

Målet är att undersöka om påståenden som ”89 % kognater mellan danska och norska” och ”82 % mellan svenska och de båda andra språken” kan bekräftas med en tydlig, reproducerbar metod.

## Varför en ny analys behövs

Olika procentsatser i litteraturen mäter olika saker. En kognatandel är inte samma sak som stavningslikhet, lexikalt avstånd eller förståelse. Resultatet påverkas också av om man räknar ordformer eller lemma, om frekvens viktas och hur sammansättningar, lånord, synonymer och falska vänner behandlas.

Tidigare studier visar att lexikalt avstånd i korta parallella texter kan vara mycket litet, men de resultaten kan inte direkt omvandlas till en procentsats för de 2 000 vanligaste orden. Se exempelvis Gooskens (2006) och Heeringa m.fl. (2014), sammanfattade i [planering/spraklig-narhet.md](../planering/spraklig-narhet.md).

## Datakällor

### Primär jämförelse: Leipzig Corpora Collection

Leipzig Corpora Collection tillhandahåller frekvensordlistor och korpusar i samma tekniska format från jämförbara källtyper. Dokumentationen skiljer bland annat mellan nyhetsmaterial, webbkällor och Wikipedia. Det gör samlingen lämplig för en jämförelse mellan språken med samma materialtyp.

Föreslagen primär datamängd:
- danska: News 2022,
- norska: News 2022,
- svenska: News 2022.

Föreslagen robusthetskontroll:
- danska, norska och svenska: Wikipedia 2021.

Språk- och korpussidor:
- [Danish](https://cls.wortschatz-leipzig.de/en?corpusLanguage=dan)
- [Norwegian](https://cls.wortschatz-leipzig.de/en?corpusLanguage=nor)
- [Swedish](https://cls.wortschatz-leipzig.de/en?corpusLanguage=swe)

Leipzig beskriver nyhetskorpusen som texter från nyhetswebbplatser och anger att korpusarna finns i jämförbara källtyper och gemensamt format. Ordlistorna innehåller ordformer med frekvenser, inte automatiskt lemmatiserade lexem. Därför måste ordforms- och lemmaanalys hållas isär.

Referens för korpusformat och jämförbara korpusar: Eckart & Quasthoff, “Statistical Corpus and Language Comparison on Comparable Corpora” (2013), beskriven på Leipzigs korpusportal.

### Kompletterande frekvensresurser

Dessa kan användas för kontroll eller alternativa analyser, men bör inte blandas in i primärresultatet utan att skillnader i korpus och metod redovisas:

- Svenska: Språkbanken Texts [Flex](https://spraakbanken.gu.se/en/resources/flex), med frekvenser från romaner, tidningar och webbforum. Licens CC BY 4.0.
- Danska: DSL:s [frekvenslista över danska lemma](https://korpus.dsl.dk/resources/details/freq-lemmas.html), baserad på BAKSPEJLET 2024 (cirka 1,1 miljarder ordformer, 1983–2024). Listan innehåller lemma och sammanlagd frekvens för böjningsformer. DSL:s användningsvillkor kräver lämplig källhänvisning och förbjuder vissa konkurrerande ordboksprodukter.
- Norskt bokmål: CLARINO Bergens [frekvensordliste fra Norsk aviskorpus](https://repo.clarino.uib.no/xmlui/handle/11509/157), 10 000 vanliga ord från elva tidningar med material från 1998–2022, CC BY 3.0. Den tillgängliga listan innehåller ordformer och behöver förbehandling innan den jämförs direkt med lemmatiserade listor.

## Tre separata mått

Resultaten ska inte sammanfattas i en enda ”likhetsprocent”.

### A. Ortografisk identitet och likhet
- Exakt identiska ordformer efter en redovisad normalisering.
- Nära stavningsformer, mätta med normaliserat Levenshtein-avstånd.
- Redovisa både före och efter en separat analys av bokstavsmotsvarigheter som æ/ä och ø/ö. Normalisering får inte radera verkliga stavningsskillnader i huvudresultatet.

### B. Kognater
Kognater är ord med gemensamt historiskt ursprung. De kan ha olika stavning och uttal. En gemensam etymologi ska inte automatiskt betyda att orden har samma moderna betydelse.

För varje jämförd ordpost ska en annotering ange:
- kognat: ja / nej / osäkert,
- betydelserelation: samma / överlappande / olika,
- relation: ärvt gemensamt ord, gemensamt lån, parallellt lån eller annan relation,
- källa och granskningsstatus.

Lånord kan räknas som etymologiskt besläktade i en bred kognatdefinition, men bör också särredovisas så att resultatet kan visas både med och utan gemensamma lån.

### C. Semantisk överensstämmelse
Mät om motsvarande ord har samma eller överlappande betydelser i modern svenska, danska och norska. Falska vänner och partiella betydelseförskjutningar ska redovisas separat.

## Urval och analysdesign

1. Använd samma korpustyp och helst samma insamlingsår för alla tre språk.
2. Hämta minst de 10 000 vanligaste ordformerna från respektive korpus så att analysen inte blir beroende av ett snävt urval.
3. Ta fram resultat för topp 500, 1 000 och 2 000.
4. Redovisa både typbaserade mått (antal olika ord) och frekvensviktade mått (hur stor andel av ordanvändningen som täcks).
5. Skilj på ordformer och lemmatiserade lexem. För lemmaanalysen ska böjningsformer grupperas med en dokumenterad metod.
6. Matcha ord mellan språken genom översättningsmotsvarigheter, inte bara genom att leta efter identiska stavningar.
7. Låt etymologiska och semantiska bedömningar granskas manuellt. Automatiska modeller får föreslå kandidater men inte ensamma fastställa kognatstatus.
8. Upprepa analysen på en annan korpusgenre, exempelvis Wikipedia, för att testa om resultaten påverkas av ämne och stil.

## Viktiga metodfrågor

- Ska norska representeras av bokmål, nynorsk eller båda? Primäranalysen bör börja med bokmål eftersom det har bred tillgång till stora jämförbara frekvensresurser. Nynorsk bör analyseras separat, inte blandas ihop med bokmål.
- Ska böjningsformer räknas som separata ord? Både ordformsresultat och lemmaresultat bör redovisas.
- Ska gemensamma internationella lånord räknas som kognater? Redovisa både bred och snäv definition.
- Hur hanteras homografer och falska vänner? Stavningslikhet och semantisk likhet måste vara separata mått.
- Hur hanteras sammansättningar? Redovisa grundord och sammansättningar separat när det är möjligt.

## Förväntad leverans

- råa frekvenslistor eller länkar, med versions- och licensuppgifter,
- normaliserade ordlistor för respektive språk,
- en gemensam annoteringstabell för ordmotsvarigheter,
- en reproducerbar analyskod,
- tabeller för 500, 1 000 och 2 000 ord,
- en rapport med metod, resultat, osäkerhet och begränsningar.

## Nuvarande slutsats

Det finns tillgängliga, öppna frekvensresurser som gör en sådan studie genomförbar. Däremot har de specifika procentsatserna 89 % och 82 % inte verifierats. De ska inte återges som fakta förrän de kan återskapas från en identifierad källa eller en ny analys.

Det första metodvalet blir att använda jämförbara nyhetskorpusar från Leipzig för huvudanalysen och Wikipedia-korpusar som robusthetskontroll. Efter att frekvenslistorna hämtats och normaliserats kan den faktiska ord-för-ord-matchningen börja.
