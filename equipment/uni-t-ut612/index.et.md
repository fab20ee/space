---
title: "Käsi-LCR-meeter UNI-T UT612"
seoDescription: "UNI-T UT612 LCR-meeter Tallinna hackspace'is: induktiivsus, mahtuvus ja takistus viiel sagedusel kuni 100 kHz, koos ESR-i, hüvetegur ja kaonurgaga."
specs:
  - { label: "Mõõdab",          value: "L, C, R, DCR ning Q, D, θ ja ESR" }
  - { label: "Testsagedused",   value: "100 Hz, 120 Hz, 1 kHz, 10 kHz, 100 kHz" }
  - { label: "Induktiivsus",    value: "20 µH – 2000 H, ±(0,5 % + 5)" }
  - { label: "Mahtuvus",        value: "200 pF – 20 mF, ±(0,5 % + 5)" }
  - { label: "Takistus",        value: "20 Ω – 200 MΩ, ±(0,3 % + 5)" }
  - { label: "Ekraan",          value: "20 000 näiduühikut, teine näit 2000 ühikut" }
  - { label: "Testsignaal",     value: "0,6 V efektiivväärtus, väljundtakistus 120 Ω" }
  - { label: "Režiimid",        value: "jada- ja rööpasendusskeem, auto-LCR, suhteline mõõtmine, sortimine hälbe järgi, kalibreerimine" }
  - { label: "Liides",          value: "USB" }
  - { label: "Toide",           value: "9 V patarei või USB" }
---

Multimeeter mõõdab kondensaatorit ühel sagedusel ja annab ühe arvu. LCR-meeter küsib, millisel
sagedusel sa seda kondensaatorit kasutada kavatsed, ja vastab juba teise arvuga. Vahe ei ole
formaalne: elektrolüüt, mis 100 Hz juures näitab oma ausat 100 µF, võib 100 kHz juures käituda nagu
takistusega traadijupp.

UT612 mõõdab induktiivsust, mahtuvust ja takistust viiel sagedusel 100 Hz-st 100 kHz-ni ning näitab
peale väärtuse enda ka seda, mis selle kõrval on: ESR, hüvetegur, kaotegur, faasinurk.

Induktiivsus väärib eraldi sõna: seda oskavad mõõta vähesed. Ükski teine seade hackspace'is
induktiivsust ei näita — ei lauamultimeeter ega käsimultimeetrid. Kui on vaja induktiivsust, on
valik täpselt üks ja see on UT612.

## Milleks seda praktikas vaja on

- **Kondensaatori ESR** on elektrolüütide peamine diagnoos. Mahtuvus võib jääda normi, aga ESR
  kasvab kümme korda ja toiteplokk hakkab vilisema ja kuumenema. Tavaline multimeeter seda ei näe.
- **Ise keritud pooli induktiivsus**: keerde on nii palju, nagu lugesid, aga induktiivsus on hoopis
  teine, sest süda ei ole see, mida arvasid.
- **Paaride sobitamine**: kaks kondensaatorit või kaks pooli sama pealekirjutatud ja erineva
  tegeliku väärtusega.
- **Sortimine** komponendikarpidest: hälberežiim näitab kõrvalekallet protsentides, mitte
  absoluutväärtust.
- **Pooli hüvetegur** tema tööagedusel — kui teed filtrit või võnkeringi, siis just see parameeter
  otsustab.

## Jadamisi või rööbiti

Meeter modelleerib detaili kahe elemendiga ja seda valikut saab ise teha. Reegel on lihtne: väikesed
mahtuvused ja suured takistused mõõdetakse rööpskeemis, suured mahtuvused ja väikesed takistused
jadaskeemis. Kui kahtled, jäta auto-LCR peale: seade saab ise aru, mis tema ees on, ja valib
mõistlikult.

## Kuidas kasutada

1. **Tühjenda kondensaator enne mõõtmist.** Seade annab oma testsignaali ega eelda, et detailis on
   energiat salvestatud. See on korpusele kirjutatud ja mitte niisama.
2. Ühenda juhtmed pesadesse „+" ja „−".
3. Vali FREQ-nupuga sagedus vastavalt ahela töösagedusele: 100 või 120 Hz võrgufiltrite jaoks,
   1 kHz üldiseks kontrolliks, 10 ja 100 kHz impulsstehnika jaoks.
4. Tee kalibreerimine: CAL lahtiste juhtmetega, seejärel lühistatud juhtmetega. See lahutab maha
   juhtmete enda mahtuvuse ja takistuse, mis väikeste väärtuste juures on kohe näha.
5. FUNC-nupuga vali, mida näidatakse teise väärtusena: D, Q, θ või ESR.
6. Paaride sobitamiseks vajuta esimese detaili järel REL; edasi näitab seade hälvet sellest.
7. Lõpus lülita välja ja pane koos juhtmetega riiulil olevasse konteinerisse tagasi.

## Mida see ei tee

See ei ole ahelas mõõtja. Detail tuleb välja joota või vähemalt üks jalg lahti tõsta, muidu mõõdad
kõike, mis plaadil temaga rööbiti on. Ja sisendpesadesse pinget anda ei tohi — seade mõõdab ise, oma
signaaliga.

## Rentimine

Selle seadme saab koju kaasa: tavaline põhjus on toiteploki või võimendi remont, kus elektrolüüte
on vaja ESR-i järgi kontrollida, ilma et peaks kogu seadme hackspace'i tassima. Päevahind ja
tähtaeg on selle lehe rendiplokis.

## Ligipääs

Seade on hackspace'i ruumis riiulil konteineris, seega on vaja hackspace'i ligipääsuga paketti.
Instruktaaži ei ole vaja.
