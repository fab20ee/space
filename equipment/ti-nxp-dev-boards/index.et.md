---
title: "TI ja NXP arendusplaadid"
seoDescription: "Texas Instrumentsi ja NXP arendusplaadid Tallinna hackspace'is: LaunchPad MSPM0L1117-ga ja FRDM-MCXN947. Et proovida midagi muud kui STM32."
specs:
  - { label: "Texas Instruments", value: "LaunchPad MSPM0L1117-ga, Arm Cortex-M0+ tuum" }
  - { label: "NXP",          value: "FRDM-MCXN947, MCX N perekond kahe Cortex-M33 tuuma ja NPU-ga" }
  - { label: "Seisund",      value: "mõlemad plaadid veel tehasekarpides, koos kaablite ja dokumentatsiooniga" }
  - { label: "Koosseis",     value: "esialgu need kaks; komplekt on mõeldud kasvama" }
---

Konteiner neile, kellel on vaja proovida midagi muud kui STM32-t.

Mikrokontrollerite tootjad on omavahel kokkusobimatud igal tasandil: perifeeria, arenduskeskkond,
silur, kellapuu seadistamise viis. Tootja valimine projekti jaoks on otsus aastateks ette ja selle
tegemine andmelehe järgi, plaati kordagi käes hoidmata, on üsna imelik. Seepärast seisavadki eri
tootjate plaadid kõrvuti.

## Mis siin on

- **TI LaunchPad MSPM0L1117-ga.** MSPM0 on Texas Instrumentsi odav Cortex-M0+ perekond, mõeldud
  lihtsate ja odavate seadmete jaoks. Keskkond on Code Composer Studio, silur on plaadi peal.
- **NXP FRDM-MCXN947.** Teine ots: MCX N perekond kahe Cortex-M33 tuuma ja riistvaralise
  närvivõrgukiirendiga. Keskkond on MCUXpresso.

Mõlemad on veel tehasekarpides, koos kaablite ja paberitega.

## Milleks see kasulik on

- Võrrelda arenduskeskkondi enne, kui valid oma projekti jaoks tootja
- Proovida seda, mida STM32-l ei ole: NXP poolel NPU, TI poolel hinnatase
- Korrata tootja näidet ilma plaati ostmata
- Saada teada, kui valus on oma koodi ühelt arhitektuurilt teisele viia — tavaliselt selgub see
  liiga hilja

Kui töötad juba STM32-ga, on kõrval [STM32 plaatide
konteiner](/et/seadmed/stm32-arendusplaadid) koos programmaatoritega.

## Komplekt on mõeldud kasvama

Praegu on see kõik, mis TI-lt ja NXP-lt olemas: üks plaat kummaltki. Loend kehtib **19. oktoobri
2026 seisuga**.

**Kui sinu projekt vajab kindlat arendusplaati, kirjuta meile.** Oleme tavaliselt valmis juurde
ostma ja enamasti ei ole sa ainus, kes seda tahab.

## Kuidas kasutada

1. Võta plaat konteinerist koos karbiga — kaabel ja dokumentatsioon on seal sees.
2. Paigalda tootja keskkond: Code Composer Studio TI jaoks, MCUXpresso NXP jaoks. Mõlemad on
   tasuta.
3. Mõlemal plaadil on silur peal, eraldi programmaatorit vaja ei ole — USB-st piisab.
4. Pane plaat karpi ja karp konteinerisse tagasi. Kaabel ka.

## Ligipääs

Konteiner asub hackspace'i ruumis, seega on vaja hackspace'i ligipääsuga paketti. Instruktaaži ei
ole vaja.
