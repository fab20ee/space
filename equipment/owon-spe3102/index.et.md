---
title: "Programmeeritav toiteplokk OWON SPE3102"
seoDescription: "Laboritoiteplokk Tallinna hackspace'is: OWON SPE3102, 0–30 V, 0–10 A, 200 W, voolupiirang, OVP- ja OCP-kaitse, tarbimise graafik ekraanil. Ligipääs 24/7."
specs:
  - { label: "Väljund",     value: "0–30 V, 0–10 A, 200 W" }
  - { label: "Lahutus",     value: "1 mV / 1 mA" }
  - { label: "Kaitse",      value: "OVP, OCP, ülekuumenemine" }
  - { label: "Ekraan",      value: "värviline 2,8\", pinge, vool ja graafik" }
  - { label: "Veel",        value: "USB 5 V / 1 A laadimiseks; arvutist juhtimine seadistamata" }
  - { label: "Juhtmed",     value: "plokis, varu on riiulil" }
---

Elektroonikalaua põhiline toiteplokk. Pinge ja voolupiir seatakse millivoldi ja milliampri
täpsusega, ja kui värskes skeemis on lühis, jääb plokk piiri peale, mitte ei lase suitsu. 10 A
jätkub mootoritele, LED-ribadele ja kütteelementidele, mitte ainult mikrokontrolleriplaatidele.
Ekraani graafik näitab, kui palju seade ajas tarbib.

## Kuidas kasutada

1. Lülita plokk sisse väljalülitatud väljundiga. Nupuga V ja nupuga sea pinge, nupuga I voolupiir.
   Piir sea nii madalale, kui skeem lubab: see päästab plaadid.
2. Soovi korral sea OVP ja OCP veidi üle tööväärtuste teiseks kaitseks.
3. Ühenda juhtmed, kontrolli polaarsust: punane pluss, must miinus, roheline klemm on maandus, mitte
   miinus. Vajuta On/Off, et väljund sisse lülitada.
4. Indikaator CC tähendab, et skeem tarbib rohkem, kui lubasid, ja plokk hoiab voolu.
5. Lõpus lülita esmalt välja väljund, siis võta juhtmed ära, siis lülita plokk välja.

## Oluline

- 10 A läbi peenikeste juhtmete või makettplaadi kuumutab need tulekahjuni. Suurte voolude jaoks
  võta korralikud juhtmed riiulilt.
- Ära ühenda väljundit pinge all oleva skeemiga ega paralleelselt teise allikaga.
- Liitiumelemente sellest ei laeta, selleks on vaja laadimisskeemi.

## Ligipääs

Plokk asub hackspace'i ruumi elektroonikalaual, vaja on hackspace'i ligipääsuga paketti. Instruktaaži
ei ole vaja. Plokk jääb ruumi.
