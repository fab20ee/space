---
title: "USB-tester FNIRSI FNB58"
seoDescription: "FNIRSI FNB58 Tallinna hackspace'is: USB-tester 4–28 V ja 7 A jaoks, kiirlaadimise protokollide tuvastuse, pulsatsiooni ja kaablitakistuse mõõtmisega."
specs:
  - { label: "Pinge",       value: "4 – 28 V" }
  - { label: "Vool",        value: "0 – 7 A" }
  - { label: "Võimsus",     value: "kuni 120 W" }
  - { label: "Pistikud",    value: "USB-A, USB-C, micro-USB — sisend ja väljund" }
  - { label: "Protokollid", value: "QC2.0/3.0, PD2.0/3.0, Huawei FCP ja SCP, Samsung AFC, VOOC ja SuperVOOC, MTK-PE" }
  - { label: "Lisaks",      value: "pulsatsioon, kaabli takistus, ampertundide ja vatt-tundide loendurid" }
  - { label: "Ekraan",      value: "2\" värviline TFT" }
  - { label: "Sees",        value: "16-bitine ADC ja eraldi PD-kiip" }
---

Tester käib laadija ja seadme vahele ning näitab, mis kaablis tegelikult toimub: pinge, vool,
võimsus ja mitu ampertundi ning vatt-tundi on läbi läinud. See vastab igapäevastele küsimustele —
miks telefon aeglaselt laeb, kas laadija räägib oma vattidest tõtt ja kas kaabel on veel elus.

Kaks asja eristavad teda lihtsast USB-testrist. Ta tuvastab kiirlaadimise protokolli, see tähendab
ütleb, milles laadija ja seade tegelikult kokku leppisid. Ja ta mõõdab kaabli takistust — just seda,
mille pärast „sama laadija" teise juhtmega laeb kaks korda aeglasemalt.

## Milleks see sobib

- Kontrollida, millise võimsuse laadija tegelikult annab, mitte mida korpusele on kirjutatud
- Leida halb kaabel: takistus ja pingelang voolu all on kohe näha
- Vaadata, milline protokoll käivitus ja millisel pingel laadija ja seade kokku leppisid
- Mõõta, kui palju energiat konkreetse seadme laadimisse läks
- Kontrollida odava toiteploki väljundi pulsatsiooni
- Uurida, mida sinu PD-laadija oskab, enne kui sellest toita [FNIRSI
  DPS-150](/et/seadmed/kaasaskantav-toiteplokk-fnirsi-dps-150)

## PD-päästiku režiim

Tester oskab ise laadijalt konkreetset pinget küsida — 9, 12, 15 või 20 V. See on mugav, et
veenduda, kas laadija tõesti annab lubatud režiimid, ja et saada tavalisest PD-laadijast vajalik
pinge.

Ohtlik osa on ilmne: **selles režiimis on liinil kuni 20 V**. Midagi kõrvalist ei tohi sel hetkel
ahelas olla — telefon, mis ootas oma viit volti, seda üle ei ela. Tootja soovitab päästiku välja
lülitatuna hoida ja sisse lülitada ainult teadlikult.

## Kuidas kasutada

1. Pane tester allika ja koormuse vahele. Sisend- ja väljundpistikud on korpusele märgitud, vaata
   nooli.
2. Loe pinget, voolu ja võimsust põhiekraanilt; energia ja aja loendurid on kõrvalekraanidel.
3. Kaabli kontrollimiseks kasuta takistuse mõõtmise režiimi: see vajab kahte mõõtmist eri voolude
   juures ja seade juhatab järjekorra ise ette.
4. Protokolli tuvastus on omaette menüüpunkt ja seade peab olema ühendatud.
5. Lülita PD-päästik sisse ainult siis, kui tead kindlalt, mis on teisel pool.

## Rentimine

Selle seadme saab koju kaasa: oma laadijaid, akupanke ja kaableid on mugavam kontrollida seal, kus
nad asuvad. Päevahind ja tähtaeg on selle lehe rendiplokis.

## Ligipääs

Tester on hackspace'i ruumis riiulil konteineris, seega on vaja hackspace'i ligipääsuga paketti.
Instruktaaži ei ole vaja.
