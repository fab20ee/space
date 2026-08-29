---
title: "Kompaktne alalisvoolu toiteplokk PCWork PCW07B"
seoDescription: "Kompaktne reguleeritav laboritoiteplokk Tallinna hackspace'is. PCWork PCW07B: 0–30 V, 0–5 A, jäme ja peen reguleerimine, LED-näidik — lihtne teine toiteallikas igapäevatööks."
specs:
  - { label: "Väljund",      value: "0–30 V, 0–5 A" }
  - { label: "Režiimid",     value: "püsipinge / püsivool" }
  - { label: "Reguleerimine", value: "vajutatavad nupud, jäme ja peen" }
  - { label: "Ekraan",       value: "LED, pinge ja vool" }
---

<!-- TODO: kontrolli voolu nimiväärtust ja lahutusvõimet andmesildi järgi; märgi, millised juhtmed
     selle juurde kuuluvad. -->

Väike, lihtne reguleeritav toiteplokk. Kaks nuppu, üks väljund, näidik — kõik, mida on vaja, et
toita mikrokontrolleriplaati, operatsioonivõimendi skeemi või andurit, kui suur OWON-i toiteplokk on
millegi muuga hõivatud. See töötab püsipinge režiimis, kuni koormus tõmbab rohkem kui seatud vool,
siis lülitub püsivoolule ja hoiab piiri.

## Milleks see sobib

- Teise skeemi toitmine laual
- Lihtsad katsed, kus 5 A on küllaga
- Fikseeritud pinge andmine plaadile, kui seda ostsilloskoobiga uurid
- „Kindlalt korras" toiteallikas plaadile, mille toites sa kahtled

## Ohutus

- Keera voolunupp enne uue skeemi ühendamist alla, siis tõsta ainult nii palju, kui skeem vajab.
- Punane on pluss, must on miinus; roheline klemm on maandus.
- Ära ühenda väljundit pinge all oleva skeemiga ega paralleelselt teise toiteallikaga.
- Ära kasuta seda liitiumelementide laadijana.

## Kuidas kasutada

1. Lülita sisse, ilma et midagi oleks ühendatud. Sea pinge jämeda ja peene nupuga.
2. Sea voolupiir: lühista väljund korraks juhtmega, keera voolunupp soovitud piirile, eemalda lühis.
   Või lihtsamalt — alusta madalalt ja tõsta, kui skeem on ühendatud.
3. Ühenda juhtmed, kontrolli polaarsust, vajuta Output.
4. Kui C.C.-indikaator põleb, tarbib skeem piirist rohkem.
5. Lõpus vajuta Output, et väljund välja lülitada, ühenda juhtmed lahti ja lülita seade välja.

## Ligipääs

Toiteplokk asub hackspace'i ruumi elektroonikalaual, seega on vaja paketti, mis sisaldab hackspace'i
ligipääsu. Ohutusinstruktaaži pole vaja.
