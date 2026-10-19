---
title: "Ostsilloskoop Tektronix TDS 794D, 2 GHz"
seoDescription: "Neljakanaliline 2 GHz ostsilloskoop Tektronix TDS 794D Tallinna hackspace'is: 4 GS/s, digitaalne fosfor. Töökoja kiireim seade kiirete frontide jaoks."
specs:
  - { label: "Ribalaius",    value: "2 GHz" }
  - { label: "Kanalid",      value: "4" }
  - { label: "Diskreetimine", value: "4 GS/s ühel kanalil, 2 GS/s kahel, 1 GS/s kolmel-neljal" }
  - { label: "ADC",          value: "8 bitti" }
  - { label: "Ekraan",       value: "sisseehitatud, tuhm — soovitame välist VGA-monitori" }
  - { label: "Liidesed",     value: "VGA, GPIB, RS-232, Centronics, 3,5\" diskett" }
---

Töökoja kiireim seade. Seal, kus [Micsig TO3004](/et/seadmed/ostsilloskoop-micsig-to3004) oma
300 MHz-ga näitab frondi asemel juba ümardatud astet, näitab TDS 794D fronti ennast — koos
võbeluse, ülelöögi ja kõige muuga, mis seal tegelikult toimub.

Seda ei ole sageli vaja, aga kui on, siis asendada ei ole millegagi. Mõnesaja pikosekundi pikkune
front, taktiliin sadade megahertside juures, peegeldus halvasti sobitatud rajas: kõik see on
olemas ainult sellise ribalaiusega seadme jaoks.

## Ekraanist

**Sisseehitatud ekraan on tuhm.** See on üheksakümnendate seade ja tema taustavalgus on oma aja ära
teeninud. Ta töötab ja selle järgi saab orienteeruda, aga terve õhtu sinna sisse piiluda ei ole
eriline nauding.

Seepärast **ühenda väline monitor VGA kaudu**. Pistik on tagapaneelil ja monitor seisab tavaliselt
kõrval riiuli peal. Pilt on seal täielik ja hele ja see lahendab küsimuse täiesti.

## Milleks see sobib

- Näha kiirete frontide tegelikku kuju, mitte nende ligikaudset siluetti
- Siluda kiireid digitaalliideseid
- Püüda lühikesi häireimpulsse, mida aeglasem seade lihtsalt ei näe
- Vaadata nelja kiiret signaali korraga
- Mõõta viiteid ja värinat mastaabis, kus loevad nanosekundid

Kõige muu jaoks võta Micsig: ta käivitub kolme sekundiga, tal on korralik ekraan ja ta ei võta
poolt lauda.

## Diskreetimissagedusest

Diskreetimissagedus jaguneb kasutatavate kanalite vahel: 4 GS/s ühel, 2 kahel, 1 kolmel või neljal.
Kõigi nelja kanali sisselülitamine siis, kui vaja on kahte, tähendab poole ajalise lahutuse
äraviskamist niisama.

## Seadme sisend

Ainus asi, mida saab sekundiga rikkuda, on sisendtrakt.

- Sellise ribalaiusega sisendite pingepiirid on palju madalamad kui tavalisel ostsilloskoobil.
  Loe enne ühendamist pistiku juures olevat märgistust.
- Võrgupinget sisendisse ei anta. Mitte kunagi ja mitte mille kaudu.
- Selle seadme otsikud ei ole Micsigi omad. Kasuta neid, mis on tema juures.
- Enne ühendamist maanda staatika: puuduta pistiku korpusega seadme kere.

## Kuidas kasutada

1. Lülita sisse ja lase soojeneda. Ta on vana ja esimesed minutid näit triivib.
2. Ühenda väline VGA-monitor, kui kavatsed töötada kauem kui viis minutit.
3. Ühenda otsik ja sea kanali menüüs jagamissuhe.
4. Autoset annab lähtepunkti, edasi keeratakse mastaapi ja käivitustaset käsitsi.
5. Lõpus lülita välja ja pane otsikud tagasi.

## Ligipääs

Ostsilloskoop asub hackspace'i ruumis, seega on vaja hackspace'i ligipääsuga paketti. Instruktaaži
ei ole vaja, aga loe sisendi osa läbi enne esimest ühendamist.
