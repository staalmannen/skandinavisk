# Hunspell-stöd för Nordum

Det här delprojektet ska ta fram stavningskontroll för Nordum i Hunspell-kompatibla program.

## Mål

Skapa och underhålla en Hunspell-ordlista och affixfil (.dic och .aff) som bygger på Nordums aktuella ordlista, stavningsregler och böjningssystem.

## Arbetsprinciper

- Nordums data och specifikation är uppströms källa.
- Befintliga svenska och danska Hunspell-ordlistor i katalogen källmaterial är jämförelsematerial, inte normerande källor för Nordums ordformer.
- Importerade källor, lokala anpassningar och genererade Hunspell-filer ska hållas åtskilda.
- Varje extern källa ska ha dokumenterad version, ursprung och licens.
- Böjningsregler ska implementeras först när de kan härledas tillräckligt säkert ur Nordums specifikation eller orddata.
- Okända eller tvetydiga former ska inte läggas in som giltiga enbart för att de förekommer i en annan skandinavisk ordlista.

## Planerade leveranser

1. Inventera Nordums ordlista, böjningsregler och tillgängliga exportformat.
2. Inventera befintligt material i källmaterial och fastställ dess licenser.
3. Definiera ett reproducerbart import- och konverteringsflöde.
4. Skapa en första .dic- och .aff-version.
5. Lägg till positiva och negativa tester för grundformer, böjningar och vanliga felstavningar.
6. Dokumentera kompatibilitet med Hunspell och program som använder formatet.

## Status

Arbetet är på planerings- och inventeringsstadiet. Befintliga filer i källmaterial är inte en färdig Nordum-ordlista och ska inte betraktas som sådan.
